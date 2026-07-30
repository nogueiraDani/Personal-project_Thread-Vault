# DESIGN_SYSTEM.md

# ThreadVault Design System

## Base

O Design System do ThreadVault é construído sobre o **Ant Design**, com
tema customizado via `ConfigProvider` e tokens alinhados à marca.

**Logo Font** - Marcellus

**Interface Font** - Inter

------------------------------------------------------------------------

# Color Tokens

## Light

  Token            Valor
  ---------------- ---------
  Primary          #6D5EF7
  Primary Hover    #5A4CE0
  Background       #FAFAFB
  Surface          #FFFFFF
  Text Primary     #1A1A1A
  Text Secondary   #6B7280
  Border           #E5E7EB
  Success          #22C55E
  Warning          #F59E0B
  Danger           #EF4444

------------------------------------------------------------------------

## Dark

  Token        Valor
  ------------ ---------
  Primary      #8B7CFF
  Background   #0F0F12
  Surface      #18181B
  Text         #F8F8F8
  Border       #27272A

------------------------------------------------------------------------

# Typography

## Marcellus

Logo 48px

H1 32px

H2 28px

------------------------------------------------------------------------

## Inter

H3 24px

Title 18px

Body 16px

Small 14px

Caption 12px

------------------------------------------------------------------------

# Radius

4 8 12 16 24

------------------------------------------------------------------------

# Spacing

4 8 12 16 24 32 48 64

------------------------------------------------------------------------

# Components

Preferir componentes do Ant Design (`Button`, `Input`, `Select`,
`Card`, `Modal`, `Drawer`, `message`/`notification`, `Skeleton`,
`Layout`, `Menu`, etc.), customizados via tema e wrappers quando
necessário.

## Inputs

-   Default
-   Focus
-   Error
-   Disabled

## Buttons

-   Primary
-   Secondary
-   Outline
-   Ghost
-   Danger

## Cards

-   Default
-   Interactive

## Feedback

-   Toast (message / notification)
-   Skeleton
-   Empty State (Empty)

## Navigation

-   Sidebar (Layout + Menu)
-   Bottom Navigation
-   Header

------------------------------------------------------------------------

# UX Guidelines

-   Mobile First
-   Touch Target \>= 44px
-   Alto contraste
-   Estados de loading
-   Estados vazios
-   Feedback imediato ao usuário
-   Transições suaves
