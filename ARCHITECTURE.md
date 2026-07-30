# ARCHITECTURE.md

# ThreadVault Architecture

## Objetivo

O ThreadVault segue uma arquitetura baseada em **Feature-Based
Architecture**, priorizando escalabilidade, reutilização e baixo
acoplamento.

------------------------------------------------------------------------

# Stack

## Frontend

-   React
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

# Estrutura

``` text
src/
├── app/
├── assets/
├── components/
├── features/
│   ├── auth/
│   ├── dashboard/
│   ├── inventory/
│   ├── profile/
│   └── threads/
├── hooks/
├── routes/
├── services/
├── store/
├── styles/
├── types/
└── utils/
```

------------------------------------------------------------------------

# Camadas

## UI

Responsável apenas pela renderização.

-   Pages
-   Layouts
-   Components

Nunca realiza chamadas HTTP diretamente.

------------------------------------------------------------------------

## Feature

Cada funcionalidade encapsula:

-   componentes
-   hooks
-   validações
-   tipos
-   serviços específicos

Exemplo:

``` text
features/
└── threads/
    ├── components/
    ├── hooks/
    ├── services/
    ├── types/
    └── pages/
```

------------------------------------------------------------------------

## Services

Comunicação com API.

Responsabilidades:

-   Axios
-   tratamento de erros
-   interceptors
-   autenticação

------------------------------------------------------------------------

## Store

Estado global utilizando Zustand.

Exemplos:

-   usuário
-   tema
-   preferências
-   filtros

Evitar armazenar dados de servidor. Para isso utilizar TanStack Query.

------------------------------------------------------------------------

## Server State

TanStack Query será responsável por:

-   cache
-   refetch
-   sincronização
-   loading
-   error state

------------------------------------------------------------------------

# Navegação

Public Routes

-   Login
-   Cadastro

Protected Routes

-   Dashboard
-   Biblioteca
-   Estoque
-   Perfil
-   Configurações

------------------------------------------------------------------------

# Fluxo de Autenticação

Login ↓ Validação (Zod) ↓ API ↓ JWT ↓ Persistência ↓ Store ↓ Protected
Routes

------------------------------------------------------------------------

# Princípios

-   Mobile First
-   Componentização
-   Separation of Concerns
-   Reutilização
-   Acessibilidade
-   Responsividade
-   Clean Code
-   Feature First
