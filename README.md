# Corretum AI — Frontend

> Sistema frontend para correção assistida por IA (projeto de TCC).

## Visão geral

Corretum AI é o frontend de um sistema de correção automática/assistida por IA para avaliações e tarefas acadêmicas. A interface foi construída com React + Vite e TypeScript, seguindo uma arquitetura em camadas (presentation, application, domain, infrastructure).

## Principais funcionalidades

- Gerenciamento de usuários (login, registro, recuperação de senha)
- Criação e gerenciamento de turmas e exames
- Envio e gerenciamento de anexos (respostas, imagens)
- Avaliação e critérios configuráveis
- Painel de estatísticas e analytics

## Tecnologias

- React 18
- TypeScript
- Vite
- Tailwind CSS
- Axios
- Zustand (state management)
- @tanstack/react-query

## Requisitos

- Node.js 18+ e npm ou Yarn
- Git

## Instalação

1. Clone o repositório

```bash
git clone https://github.com/Maycon-M/frontend-ai-grading-system.git
cd frontend-ai-grading-system
```

2. Instale dependências

```bash
npm install
# ou
yarn
```

## Scripts úteis

Execute os comandos a partir da raiz do projeto.

- Desenvolvimento (hot-reload):

```bash
npm run dev
```

- Build de produção:

```bash
npm run build
```

- Inspeção/lint:

```bash
npm run lint
```

- Preview do build:

```bash
npm run preview
```

## Estrutura do projeto (resumo)

- `src/`
  - `application/` — casos de uso, lógica de aplicação
  - `domain/` — entidades, modelos, contratos (interfaces)
  - `infrastructure/` — implementações de repositórios, serviços, cliente HTTP
  - `presentation/` — componentes React, hooks e páginas
  - `main.tsx` / `App.tsx` — ponto de entrada

Outras pastas/arquivos importantes:

- `docker/` — Dockerfile para containerização
- `vite.config.ts`, `tsconfig.json`, `tailwind.config.js`

## Docker

Há um `docker/Dockerfile` com configuração base para construir a imagem do frontend. Ajuste conforme necessário para integração com backend e CI/CD.
