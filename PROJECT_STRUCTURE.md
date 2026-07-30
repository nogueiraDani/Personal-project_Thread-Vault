# PROJECT_STRUCTURE.md

# ThreadVault - Project Structure

## Stack

### Frontend

-   React 19
-   TypeScript
-   Vite
-   React Router
-   Ant Design
-   TanStack Query
-   Zustand
-   React Hook Form
-   Zod
-   Axios
-   Framer Motion

------------------------------------------------------------------------

## Estrutura de Pastas

``` text
src/
│
├── app/
├── assets/
│   ├── fonts/
│   ├── icons/
│   └── images/
│
├── components/
│   ├── ui/
│   ├── layout/
│   └── common/
│
├── features/
│   ├── auth/
│   ├── dashboard/
│   ├── threads/
│   ├── inventory/
│   └── profile/
│
├── hooks/
├── services/
├── store/
├── contexts/
├── routes/
├── types/
├── utils/
├── styles/
├── constants/
└── main.tsx
```

------------------------------------------------------------------------

## Convenções

-   Componentes: PascalCase
-   Hooks: useNomeHook.ts
-   Interfaces: IThread
-   Types: Thread.ts
-   Pastas em lowercase
-   Um componente por arquivo

------------------------------------------------------------------------

## Git Flow

main develop feature/* fix/* hotfix/\*

------------------------------------------------------------------------

## Conventional Commits

feat: fix: docs: style: refactor: test: build: chore:

------------------------------------------------------------------------

## Princípios

-   Mobile First
-   Componentização
-   Clean Code
-   SOLID quando aplicável
-   Acessibilidade
-   Responsividade
-   Design System First
