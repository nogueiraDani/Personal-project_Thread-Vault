# COMPONENT_GUIDELINES.md

# Component Guidelines

## Objetivo

Documentar padrões para criação e utilização dos componentes do Design
System.

------------------------------------------------------------------------

# Regras Gerais

Todos os componentes devem:

-   Ser reutilizáveis
-   Receber props tipadas
-   Possuir estados de loading
-   Possuir estados disabled
-   Possuir foco acessível
-   Seguir o tema da aplicação
-   Ser documentados

------------------------------------------------------------------------

# Button

## Props

-   variant
-   size
-   loading
-   disabled
-   icon
-   fullWidth
-   onClick

## Variants

-   primary
-   secondary
-   outline
-   ghost
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

## Estados

-   default
-   focus
-   error
-   disabled

## Deve possuir

-   label
-   helper text
-   mensagem de erro
-   suporte ao React Hook Form

------------------------------------------------------------------------

# Card

Utilizar para agrupar informações relacionadas.

Nunca utilizar apenas para criar espaçamento.

------------------------------------------------------------------------

# Dialog

Sempre possuir:

-   título
-   descrição opcional
-   botão cancelar
-   botão confirmar

------------------------------------------------------------------------

# Toast

Tipos:

-   success
-   info
-   warning
-   error

Tempo padrão:

3 segundos

------------------------------------------------------------------------

# Empty State

Todo módulo deve possuir um estado vazio contendo:

-   ilustração
-   título
-   descrição
-   CTA

------------------------------------------------------------------------

# Skeleton

Utilizar enquanto dados estão sendo carregados.

Nunca substituir por spinner em listas.

------------------------------------------------------------------------

# Sidebar

Desktop apenas.

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

-   Reutilizável?
-   Tipado?
-   Responsivo?
-   Testável?
-   Acessível?
-   Documentado?
-   Segue o tema?
