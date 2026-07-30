# COMPONENT_GUIDELINES.md

# Component Guidelines

## Objetivo

Documentar padrões para criação e utilização dos componentes do Design
System, preferencialmente baseados no **Ant Design**.

------------------------------------------------------------------------

# Regras Gerais

Todos os componentes devem:

-   Preferir componentes do Ant Design quando cobrirem o caso de uso
-   Ser reutilizáveis (wrappers tipados quando necessário)
-   Receber props tipadas
-   Possuir estados de loading
-   Possuir estados disabled
-   Possuir foco acessível
-   Seguir o tema da aplicação (`ConfigProvider`)
-   Ser documentados

------------------------------------------------------------------------

# Button

Base: `Button` do Ant Design.

## Props

-   variant / type
-   size
-   loading
-   disabled
-   icon
-   fullWidth / block
-   onClick

## Variants

-   primary
-   secondary / default
-   outline / dashed
-   ghost / text
-   danger

## Sizes

-   sm
-   md
-   lg

## Quando usar

-   Ações principais
-   Confirmações
-   Navegação

## Evitar

-   Links simples
-   Ações destrutivas sem confirmação

------------------------------------------------------------------------

# Input

Base: `Input` / `Input.Password` do Ant Design.

## Estados

-   default
-   focus
-   error
-   disabled

## Deve possuir

-   label (`Form.Item`)
-   helper text
-   mensagem de erro
-   suporte ao React Hook Form

------------------------------------------------------------------------

# Card

Base: `Card` do Ant Design.

Utilizar para agrupar informações relacionadas.

Nunca utilizar apenas para criar espaçamento.

------------------------------------------------------------------------

# Dialog

Base: `Modal` do Ant Design.

Sempre possuir:

-   título
-   descrição opcional
-   botão cancelar
-   botão confirmar

------------------------------------------------------------------------

# Toast

Base: `message` ou `notification` do Ant Design.

Tipos:

-   success
-   info
-   warning
-   error

Tempo padrão:

3 segundos

------------------------------------------------------------------------

# Empty State

Base: `Empty` do Ant Design.

Todo módulo deve possuir um estado vazio contendo:

-   ilustração
-   título
-   descrição
-   CTA

------------------------------------------------------------------------

# Skeleton

Base: `Skeleton` do Ant Design.

Utilizar enquanto dados estão sendo carregados.

Nunca substituir por spinner em listas.

------------------------------------------------------------------------

# Sidebar

Desktop apenas.

Base: `Layout.Sider` + `Menu` do Ant Design.

Deve permitir:

-   colapsar
-   destacar rota ativa
-   navegação por teclado

------------------------------------------------------------------------

# Bottom Navigation

Mobile apenas.

Máximo de cinco itens.

------------------------------------------------------------------------

# Convenções

## Componentes

PascalCase

Exemplo

Button.tsx

------------------------------------------------------------------------

## Hooks

useNomeHook.ts

------------------------------------------------------------------------

## Props

Sempre criar interfaces explícitas.

Evitar any.

------------------------------------------------------------------------

# Acessibilidade

-   Navegação por teclado
-   Focus visível
-   Contraste adequado
-   Labels em formulários
-   aria-\* quando necessário

------------------------------------------------------------------------

# Checklist antes de criar um componente

-   Já existe no Ant Design?
-   Reutilizável?
-   Tipado?
-   Responsivo?
-   Testável?
-   Acessível?
-   Documentado?
-   Segue o tema?
