# TecBoard - Plataforma de Eventos

Este é um projeto Next.js que demonstra o uso de Server Components e Client Components com json-server.

## Tecnologias Utilizadas

- **Next.js 15** com App Router
- **React 19** 
- **TailwindCSS** para estilização
- **json-server** para simulação de API
- **pnpm** como gerenciador de pacotes

## Estrutura do Projeto

### Server Component
- `EventsList.js` - Busca dados do json-server no lado do servidor

### Client Component  
- `EventCard.js` - Componente interativo com estado local (botão de curtir)

## Como executar

1. **Instalar dependências:**
```bash
pnpm install
```

2. **Executar o json-server em um terminal:**
```bash
pnpm run json-server
```
Isso iniciará a API mock na porta 3001 com os dados do `db.json`.

3. **Executar a aplicação Next.js em outro terminal:**
```bash
pnpm run dev
```
A aplicação estará disponível em [http://localhost:3000](http://localhost:3000).

## Funcionalidades

- **Listagem de eventos:** Os dados são buscados do json-server no servidor
- **Interatividade:** Cada card de evento possui um botão de curtir funcional
- **Responsividade:** Layout adaptável para diferentes tamanhos de tela
- **Loading states:** Tratamento de erros e estados de carregamento

## API Endpoints

- `GET /events` - Lista todos os eventos

## Scripts Disponíveis

- `pnpm run dev` - Executa a aplicação em modo desenvolvimento
- `pnpm run build` - Gera build de produção
- `pnpm run start` - Executa a aplicação em modo produção
- `pnpm run json-server` - Inicia o json-server na porta 3001
- `pnpm run lint` - Executa o linter (Biome)
- `pnpm run format` - Formata o código (Biome)
