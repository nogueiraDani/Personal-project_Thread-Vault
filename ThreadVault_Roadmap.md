# ThreadVault --- Roadmap de Desenvolvimento

> Objetivo: desenvolver um projeto completo para evoluir conhecimentos
> em **React + TypeScript + Design System**, seguindo uma abordagem
> **Mobile First**, com foco em arquitetura de frontend e boas práticas.

---

# Fase 0 --- UX/UI & Product Discovery

## Objetivo

Definir toda a identidade visual e experiência do usuário antes de
iniciar a implementação.

### Etapas

- Definir identidade da marca
- Criar logo
- Definir paleta de cores
- Escolher tipografia (Marcellus + Inter)
- Definir ícones
- Criar wireframes
- Criar protótipo navegável
- Validar fluxo de navegação

### Entrega

- Protótipo aprovado
- Design System definido

---

# Fase 1 --- Project Setup

## Objetivo

Preparar toda a infraestrutura do projeto.

### Etapas

- Criar repositório no GitHub
- Configurar GitHub Projects (Kanban)
- Criar README inicial
- Criar projeto React + Vite + TypeScript
- Configurar ESLint
- Configurar Prettier
- Configurar Husky
- Configurar aliases
- Configurar Tailwind CSS
- Instalar React Router
- Organizar estrutura de pastas

### Entrega

- Projeto inicial funcionando
- Estrutura pronta para desenvolvimento

---

# Fase 2 --- Design System

## Objetivo

Construir uma biblioteca reutilizável de componentes.

### Foundations

- Colors
- Typography
- Spacing
- Radius
- Shadows
- Breakpoints
- Icons

### Componentes Base

- Button
- IconButton
- Input
- PasswordInput
- Checkbox
- Switch
- Select
- Badge
- Chip
- Divider

### Componentes Compostos

- Card
- Dialog
- Drawer
- Sidebar
- Bottom Navigation
- Header
- SearchBar
- Empty State
- Skeleton
- Toast

### Extras

- Light Theme
- Dark Theme
- Estados (hover, focus, disabled)
- Micro animações

### Entrega

- Design System completo

---

# Fase 3 --- Layout da Aplicação

## Objetivo

Construir a estrutura visual do aplicativo.

### Telas

- Splash
- Login
- Cadastro
- Dashboard
- Biblioteca
- Cadastro de Linha
- Detalhes da Linha
- Estoque
- Perfil
- Configurações

### Layout

- Mobile First
- Sidebar Desktop
- Bottom Navigation
- Floating Action Button
- Header

### Entrega

- Navegação funcional
- Layout responsivo

---

# Fase 4 --- Autenticação

## Objetivo

Implementar autenticação e gerenciamento de sessão.

### Etapas

- React Hook Form
- Zod
- Login
- Cadastro
- Persistência de sessão
- Zustand ou Context API
- Protected Routes

### Entrega

- Fluxo de autenticação funcionando

---

# Fase 5 --- Biblioteca de Linhas

## Objetivo

Criar a principal funcionalidade do aplicativo.

### Etapas

- Modelo Thread
- Lista de linhas
- Cards
- Favoritos
- Quantidade
- Tenho / Não tenho
- Localização

### Entrega

- Biblioteca funcional

---

# Fase 6 --- Cadastro de Linhas

## Objetivo

Implementar o CRUD completo.

### Campos

- Código
- Marca
- Nome
- Quantidade
- Cor
- Categoria
- Observações

### Recursos

- Preview da cor
- Validação
- Feedback visual

### Entrega

- CRUD completo

---

# Fase 7 --- Dashboard

## Objetivo

Criar uma visão geral da coleção.

### Widgets

- Total de linhas
- Tenho
- Não tenho
- Favoritas
- Baixo estoque
- Últimas adicionadas
- Progresso da coleção

### Entrega

- Dashboard completo

---

# Fase 8 --- Busca & Filtros

## Objetivo

Melhorar a experiência de consulta.

### Busca

- Código
- Nome
- Marca

### Filtros

- Marca
- Categoria
- Favoritas
- Tenho
- Não tenho

### Ordenação

- Código
- Nome
- Quantidade

### Entrega

- Sistema de busca e filtros completo

---

# Fase 9 --- Persistência

## Objetivo

Persistir os dados da aplicação.

### Evolução

1.  LocalStorage
2.  JSON Server
3.  API Node.js

### Entrega

- Dados persistentes

---

# Fase 10 --- Backend

## Objetivo

Criar uma API REST para a aplicação.

### Stack

- Node.js
- Express
- Prisma
- PostgreSQL

### Funcionalidades

- Login
- CRUD
- JWT
- Upload de imagens

### Entrega

- API integrada ao frontend

---

# Fase 11 --- Deploy

## Objetivo

Publicar a aplicação.

### Serviços

- Frontend: Vercel
- Backend: Railway ou Render
- Banco: Neon

### Entrega

- Aplicação online

---

# Fase 12 --- Refinamentos

## Objetivo

Elevar a qualidade do projeto.

### UX

- Skeleton
- Loading
- Empty State
- Error State

### Performance

- Lazy Loading
- Code Splitting
- Memoization
- TanStack Query

### Qualidade

- Testes
- Error Boundary
- Acessibilidade
- Lighthouse

### Entrega

- Projeto pronto para portfólio profissional
