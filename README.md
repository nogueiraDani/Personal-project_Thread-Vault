# ThreadVault

Aplicação web para organizar e gerenciar uma coleção de linhas (código, marca, cor, quantidade e estoque), com foco em **React + TypeScript + Design System**, arquitetura de frontend e abordagem **Mobile First**.

> Projeto de estudo voltado a boas práticas, componentização e evolução até um portfólio profissional completo (frontend + API + deploy).

---

## Objetivo

Desenvolver um produto completo, da descoberta de UX/UI ao deploy, praticando:

- Design System reutilizável
- Feature-Based Architecture
- Autenticação e rotas protegidas
- CRUD, busca e filtros
- Persistência local → API REST
- Performance, acessibilidade e testes

---

## Stack

### Frontend

| Tecnologia | Uso |
| --- | --- |
| React 19 | UI |
| TypeScript | Tipagem |
| Vite | Bundler / dev server |
| React Router | Navegação |
| Ant Design | Biblioteca de componentes e Design System |
| TanStack Query | Server state (cache, loading, sync) |
| Zustand | Estado global (usuário, tema, preferências) |
| React Hook Form + Zod | Formulários e validação |
| Axios | Cliente HTTP |
| Framer Motion | Micro animações |

### Backend (planejado)

- Node.js + Express
- Prisma + PostgreSQL
- JWT
- Upload de imagens

### Deploy (planejado)

- Frontend: Vercel
- Backend: Railway ou Render
- Banco: Neon

---

## Funcionalidades

- **Autenticação** — login, cadastro, sessão e rotas protegidas
- **Biblioteca de linhas** — listagem, cards, favoritos, quantidade, localização, status tenho / não tenho
- **CRUD de linhas** — código, marca, nome, quantidade, cor, categoria e observações
- **Dashboard** — totais, favoritas, baixo estoque, últimas adicionadas e progresso da coleção
- **Busca e filtros** — por código, nome, marca, categoria e ordenação
- **Layout responsivo** — Sidebar (desktop), Bottom Navigation (mobile), Header e FAB

---

## Arquitetura

O projeto segue **Feature-Based Architecture**: cada domínio encapsula componentes, hooks, validações, tipos e serviços.

```text
src/
├── app/
├── assets/
├── components/          # ui / layout / common
├── features/
│   ├── auth/
│   ├── dashboard/
│   ├── inventory/
│   ├── profile/
│   └── threads/
├── hooks/
├── routes/
├── services/            # Axios, interceptors, erros
├── store/               # Zustand (não usar para dados de servidor)
├── styles/
├── types/
└── utils/
```

### Camadas

| Camada | Responsabilidade |
| --- | --- |
| **UI** | Páginas, layouts e componentes — sem chamadas HTTP |
| **Feature** | Domínio isolado (components, hooks, services, types, pages) |
| **Services** | Comunicação com API |
| **Store** | Estado global (usuário, tema, filtros) |
| **Server State** | Cache e sincronização via TanStack Query |

### Princípios

Mobile First · Componentização · Separation of Concerns · Acessibilidade · Responsividade · Clean Code · Feature First · Design System First

Detalhes em [ARCHITECTURE.md](./ARCHITECTURE.md) e [PROJECT_STRUCTURE.md](./PROJECT_STRUCTURE.md).

---

## Design System

Baseado no **Ant Design**, com tema customizado via `ConfigProvider`.

| Token | Valor |
| --- | --- |
| Logo | Marcellus |
| Interface | Inter |
| Primary (light) | `#6D5EF7` |
| Background (light) | `#FAFAFB` |
| Primary (dark) | `#8B7CFF` |
| Background (dark) | `#0F0F12` |

Fundações: tokens de tema, tipografia, spacing, radius, shadows, breakpoints e temas light/dark.

Componentes: preferir Ant Design (`Button`, `Input`, `Select`, `Card`, `Modal`, `Drawer`, `Skeleton`, `Layout`, etc.), com wrappers tipados quando necessário.

Diretrizes em [DESIGN_SYSTEM.md](./DESIGN_SYSTEM.md) e [COMPONENT_GUIDELINES.md](./COMPONENT_GUIDELINES.md).

---

## Roadmap

| Fase | Foco |
| --- | --- |
| 0 | UX/UI & Product Discovery |
| 1 | Project Setup (Vite, ESLint, Prettier, Husky, Ant Design) |
| 2 | Design System |
| 3 | Layout da aplicação |
| 4 | Autenticação |
| 5 | Biblioteca de linhas |
| 6 | Cadastro / CRUD |
| 7 | Dashboard |
| 8 | Busca & filtros |
| 9 | Persistência (LocalStorage → JSON Server → API) |
| 10 | Backend (Express + Prisma + PostgreSQL) |
| 11 | Deploy |
| 12 | Refinamentos (testes, performance, a11y, Lighthouse) |

Roadmap completo: [ThreadVault_Roadmap.md](./ThreadVault_Roadmap.md) · Backlog: [BACKLOG.md](./BACKLOG.md)

---

## Status atual

O repositório está na etapa de documentação e discovery (Fase 0 / início da Fase 1). A implementação do app React ainda será iniciada.

---

## Convenções

- **Componentes:** PascalCase (`Button.tsx`)
- **Hooks:** `useNomeHook.ts`
- **Interfaces:** `IThread` · **Types:** `Thread.ts`
- **Pastas:** lowercase · um componente por arquivo
- **Commits:** [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, …)
- **Branches:** `main` · `develop` · `feature/*` · `fix/*` · `hotfix/*`

---

## Documentação

| Documento | Conteúdo |
| --- | --- |
| [ARCHITECTURE.md](./ARCHITECTURE.md) | Stack, camadas e fluxo de auth |
| [PROJECT_STRUCTURE.md](./PROJECT_STRUCTURE.md) | Pastas e convenções |
| [DESIGN_SYSTEM.md](./DESIGN_SYSTEM.md) | Tokens, tipografia e UX |
| [COMPONENT_GUIDELINES.md](./COMPONENT_GUIDELINES.md) | Padrões de componentes |
| [ThreadVault_Roadmap.md](./ThreadVault_Roadmap.md) | Fases de desenvolvimento |
| [BACKLOG.md](./BACKLOG.md) | Product backlog por milestone |

---

## Licença

Uso educacional / portfólio. Defina a licença do repositório conforme preferir.
