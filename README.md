![Tecboard](.github/thumbnail.png)

# Tecboard - Hub de Eventos de Tecnologia

Aplicação web desenvolvida em **Next.js** para visualizar eventos de tecnologia. O projeto demonstra conceitos modernos do Next.js como Server Components, Client Components e renderização híbrida.

## 🔨 Funcionalidades do projeto

A aplicação oferece as seguintes funcionalidades:

- **Listagem de eventos**: Visualização de eventos em cards com imagem, nome, data e tema
- **Server Components**: Busca de dados no servidor para melhor performance
- **Client Components**: Interatividade com funcionalidade de curtir eventos
- **Interface responsiva**: Design moderno com Tailwind CSS
- **Otimização de imagens**: Uso do componente Image do Next.js

## ✔️ Técnicas e tecnologias utilizadas

As principais tecnologias e bibliotecas utilizadas no projeto:

- `Next.js 15.5.2`: Framework React com renderização híbrida
- `React 19.1.0`: Biblioteca para construção da interface
- `Tailwind CSS 4`: Framework CSS utilitário para estilização
- `JSON Server`: API mock para desenvolvimento
- `Biome`: Ferramenta moderna para linting e formatação de código
- `Turbopack`: Build tool ultra-rápido do Next.js

## 🎯 Conceitos do Next.js implementados

### Server Components
- **EventsList**: Componente do servidor que busca dados da API
- Renderização no servidor para melhor SEO e performance inicial
- Uso de `fetch` com `cache: 'no-store'` para dados sempre atualizados

### Client Components  
- **EventCard**: Componente do cliente com estado para interatividade
- Funcionalidade de curtir eventos com estado local
- Uso da diretiva `"use client"` para habilitar hooks do React

### Otimizações
- Componente `Image` do Next.js para otimização automática de imagens
- Estilização responsiva com Tailwind CSS
- Estrutura de projeto organizada em componentes reutilizáveis

## 📁 Acesso ao projeto

Você pode acessar o código fonte do projeto neste repositório ou fazer o download/clone para sua máquina local.

## 🛠️ Abrir e rodar o projeto

Após baixar o projeto, siga os passos abaixo:

### Pré-requisitos
- Node.js (versão 18 ou superior)
- pnpm (gerenciador de pacotes)

### Instalação

1. **Clone o repositório** (se ainda não fez):
```bash
git clone <url-do-repositorio>
cd 4874-tecboard-nextjs
```

2. **Instale as dependências**:
```bash
pnpm install
```

3. **Execute o servidor JSON (API mock)**:
```bash
pnpm run json-server
```

4. **Em outro terminal, execute a aplicação**:
```bash
pnpm run dev
```

5. **Acesse a aplicação**:
Abra seu navegador e vá para `http://localhost:3000`

### Scripts disponíveis

- `pnpm run dev` - Inicia o servidor de desenvolvimento com Turbopack
- `pnpm run build` - Gera a build de produção
- `pnpm run start` - Inicia o servidor de produção
- `pnpm run lint` - Executa o linting do código com Biome
- `pnpm run format` - Formata o código com Biome
- `pnpm run json-server` - Inicia o JSON Server na porta 3001

## 🌐 API

O projeto utiliza JSON Server para simular uma API REST. Os dados dos eventos ficam armazenados no arquivo `db.json` e a API roda na porta 3001.

**Endpoints disponíveis:**
- `GET /events` - Lista todos os eventos

**Estrutura dos dados:**
```json
{
  "events": [
    {
      "id": "1",
      "name": "Workshop React",
      "theme": "Front-end", 
      "date": "2025-05-20",
      "image": "https://placehold.co/236x282"
    }
  ]
}
```

## 📚 Mais informações do curso

Este projeto foi desenvolvido como parte do curso da Alura sobre Next.js, abordando conceitos modernos de desenvolvimento frontend como:

- Server Components e Client Components
- Renderização híbrida (SSR/CSR)
- Otimização de performance com Next.js
- Design responsivo com Tailwind CSS
- Boas práticas de desenvolvimento moderno

Gostou do projeto e quer conhecer mais? Você pode acessar o curso da Alura que desenvolve este projeto!

## 🏗️ Estrutura do projeto

```
src/
  app/
    favicon.ico
    globals.css      # Estilos globais com Tailwind
    layout.js        # Layout raiz da aplicação
    page.js          # Página inicial
  components/
    EventCard.js     # Client Component - Card de evento
    EventsList.js    # Server Component - Lista de eventos
```

O projeto segue a estrutura do App Router do Next.js 13+, separando claramente Server Components e Client Components para otimizar a performance e experiência do usuário.
