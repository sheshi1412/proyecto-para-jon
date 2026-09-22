---
version: alpha
name: Espinosa Bazet Sherdi Sebastian
description: Sistema de diseño moderno y minimalista con tonalidades carmesíes y negras para transmitir elegancia y sobriedad.
colors:
  primary: "#C41E3A"
  primaryDark: "#950606"
  neutralDark: "#000000"
  neutralLight: "#FFFFFF"
  background: "{colors.neutralLight}"
  surface: "{colors.neutralLight}"
  onPrimary: "{colors.neutralLight}"
  onSurface: "{colors.neutralDark}"
  border: "{colors.neutralDark}"
typography:
  displayLarge:
    fontFamily: "Olana"
    fontSize: "45px"
    fontWeight: 400
    lineHeight: "48px"
    letterSpacing: "0px"
  displayMedium:
    fontFamily: "Olana"
    fontSize: "40px"
    fontWeight: 400
    lineHeight: "48px"
    letterSpacing: "0px"
  displayMobile:
    fontFamily: "Olana"
    fontSize: "32px"
    fontWeight: 400
    lineHeight: "40px"
    letterSpacing: "0px"
  subtitle:
    fontFamily: "Moranga"
    fontSize: "25px"
    fontWeight: 400
    lineHeight: "32px"
    letterSpacing: "0px"
  bodyLarge:
    fontFamily: "Helvetica"
    fontSize: "20px"
    fontWeight: 400
    lineHeight: "28px"
    letterSpacing: "0px"
  bodyMedium:
    fontFamily: "Helvetica"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: "1.0"
    letterSpacing: "0px"
  bodySmall:
    fontFamily: "Helvetica"
    fontSize: "12px"
    fontWeight: 400
    lineHeight: "1.0"
    letterSpacing: "0px"
  link:
    fontFamily: "Times New Roman"
    fontSize: "10px"
    fontWeight: 400
    lineHeight: "1.0"
    letterSpacing: "0px"
rounded:
  none: "0px"
  subtle: "8px"
  special: "15px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "48px"
  xxl: "64px"
  marginMobile: "24px"
  marginDesktop: "64px"
  gutterMobile: "16px"
  gutterDesktop: "24px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.onPrimary}"
    typography: "{typography.bodyLarge}"
    rounded: "{rounded.none}"
    padding: "{spacing.sm} {spacing.md}"
    size: "auto"
  button-primary-hover:
    backgroundColor: "{colors.primaryDark}"
    textColor: "{colors.onPrimary}"
    typography: "{typography.bodyLarge}"
    rounded: "{rounded.none}"
    padding: "{spacing.sm} {spacing.md}"
    size: "auto"
  button-floating:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.onPrimary}"
    typography: "{typography.bodyLarge}"
    rounded: "{rounded.special}"
    padding: "{spacing.md} {spacing.lg}"
    size: "auto"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
    size: "auto"
  card-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
    size: "auto"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.none}"
    padding: "{spacing.sm} {spacing.md}"
    size: "auto"
  modal:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.subtle}"
    padding: "{spacing.lg}"
    size: "auto"
  popover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.subtle}"
    padding: "{spacing.md}"
    size: "auto"
  dropdown:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.subtle}"
    padding: "{spacing.md}"
    size: "auto"
  toast:
    backgroundColor: "{colors.neutralDark}"
    textColor: "{colors.neutralLight}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.subtle}"
    padding: "{spacing.md} {spacing.lg}"
    size: "auto"
  link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.link}"
    rounded: "{rounded.none}"
    padding: "0"
    size: "auto"
  navigation:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.onSurface}"
    typography: "{typography.bodyMedium}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
    size: "auto"
  divider:
    backgroundColor: "{colors.border}"
    textColor: "{colors.neutralLight}"
    typography: "{typography.bodySmall}"
    rounded: "{rounded.none}"
    padding: "0"
    size: "auto"
---

# Overview

Este documento define el sistema de diseño de la marca **Espinosa Bazet Sherdi Sebastian**. La marca proyecta una estética **moderna y minimalista**, fácil de comprender para la audiencia, utilizando tonalidades carmesíes y negras para transmitir **elegancia y sobriedad**.

El sistema se basa en:
- Una paleta de 4 colores con contraste óptimo
- 4 familias tipográficas con jerarquía estricta
- Sistema de espaciado en múltiplos de 8px
- Diseño plano (flat) con elevaciones funcionales
- Bordes rectos por defecto (0px)
- Componentes con estados bien definidos

---

## Colors

La paleta está compuesta por **cuatro tonos** que aseguran un contraste óptimo en las composiciones:

| Token | Valor | Uso |
|-------|-------|-----|
| `colors.primary` | `#C41E3A` | Rojo Carmesí ajustado — color principal de marca, botones primarios, acentos (contraste 4.5:1 vs blanco) |
| `colors.primaryDark` | `#950606` | Rojo Oscuro — estados hover/active, focus rings, overlay botón flotante |
| `colors.neutralDark` | `#000000` | Negro — texto principal, bordes, fondos oscuros |
| `colors.neutralLight` | `#FFFFFF` | Blanco — fondos, superficies, texto sobre oscuro |

**Tokens semánticos derivados:**
- `colors.background` → `{colors.neutralLight}`
- `colors.surface` → `{colors.neutralLight}`
- `colors.onPrimary` → `{colors.neutralLight}`
- `colors.onSurface` → `{colors.neutralDark}`
- `colors.border` → `{colors.neutralDark}`

> **Regla**: Usar blanco (`#FFFFFF`) para garantizar contraste adecuado sobre fondos u elementos oscuros.

---

## Typography

Se emplean **cuatro familias tipográficas** para estructurar la jerarquía visual del contenido:

| Familia | Token(es) | Uso exclusivo |
|---------|-----------|---------------|
| **Olana** | `typography.displayLarge`, `displayMedium`, `displayMobile` | Títulos principales (45px / 40px / 32px móvil) — solo alta importancia |
| **Moranga** | `typography.subtitle` | Subtítulos (25px) — **reservada estrictamente** |
| **Helvetica** | `typography.bodyLarge`, `bodyMedium`, `bodySmall` | Cuerpo de texto (15px), textos secundarios (12px), etiquetas de botones (20px), navegación |
| **Times New Roman** | `typography.link` | Enlaces (10px) con subrayado estándar |

**Tokens tipográficos completos:**

| Token | Tamaño | Interlineado | Peso | Fuente | Uso |
|-------|--------|--------------|------|--------|-----|
| `displayLarge` | 45px | 48px | 400 | Olana | Títulos principales máx. jerarquía |
| `displayMedium` | 40px | 48px | 400 | Olana | Títulos principales secundarios |
| `displayMobile` | 32px | 40px | 400 | Olana | Títulos principales en móvil |
| `subtitle` | 25px | 32px | 400 | Moranga | Subtítulos exclusivamente |
| `bodyLarge` | 20px | 28px | 400 | Helvetica | Etiquetas de botones |
| `bodyMedium` | 15px | 1.0 | 400 | Helvetica | Cuerpo de texto principal |
| `bodySmall` | 12px | 1.0 | 400 | Helvetica | Textos secundarios/pequeños |
| `link` | 10px | 1.0 | 400 | Times New Roman | Enlaces (subrayado) |

**Reglas obligatorias:**
- ❌ No aplicar opacidad a ninguna tipografía
- ❌ No usar Moranga para cuerpo de texto ni títulos principales
- ❌ No usar Olana fuera de títulos principales
- ❌ No usar Times New Roman fuera de enlaces

---

## Layout

Sistema flexible basado en una **unidad base de 8px** (`spacing.xs` = 8px).

**Espaciado (múltiplos de 8px):**
- `spacing.xs` = 8px
- `spacing.sm` = 16px
- `spacing.md` = 24px
- `spacing.lg` = 32px
- `spacing.xl` = 48px
- `spacing.xxl` = 64px

**Márgenes exteriores:**
- Móvil: 24px (`spacing.marginMobile`)
- Escritorio: 64px (`spacing.marginDesktop`)

**Gutters (separación de columnas):**
- Móvil: 16px (`spacing.gutterMobile`)
- Escritorio: 24px (`spacing.gutterDesktop`)

**Alineación:** Texto alineado a la izquierda, **evitando justificación**.

**Retícula:** Adaptativa, una columna en móvil, múltiples columnas en escritorio aprovechando márgenes amplios.

---

## Elevation & Depth

El diseño mantiene una **base plana (flat design)** con elevaciones funcionales para generar jerarquía visual:

| Nivel | Sombra | Uso |
|-------|--------|-----|
| Base plana | Sin sombra | Tarjetas en reposo, campos, navegación |
| Sutil | `0 2px 4px rgba(0,0,0,0.12)` | Hover de tarjetas (`card-hover`) |
| Media | `0 4px 12px rgba(0,0,0,0.12)` | Tarjetas elevadas, modales, popovers |
| Alta | `0 8px 24px rgba(0,0,0,0.15)` | Botones flotantes + velo rojo oscuro 90% opacidad |
| Alta exclusiva | `0 8px 24px rgba(0,0,0,0.16)` | Menús desplegables principales, modales flotantes, toasts fijos |

**Regla general:** Mantener bordes definidos y evitar capas múltiples de sombras para preservar la estética sobria.

---

## Shapes

| Token | Valor | Uso |
|-------|-------|-----|
| `rounded.none` | 0px | Configuración por defecto — estilo limpio y moderno |
| `rounded.subtle` | 8px | Opcional para elementos flotantes |
| `rounded.special` | 15px | Exclusivo para componentes especiales |

**Isotipo / Logo:** `assets/ilustración_sherdi_pp.jpg` — motivo gráfico principal de la marca.

---

## Components

### Botones
- **`button-primary`**: Fondo `{colors.primary}`, texto `{colors.onPrimary}`, tipografía `{typography.bodyLarge}`, bordes `{rounded.none}`, padding `{spacing.sm} {spacing.md}`
- **`button-primary-hover`**: Fondo `{colors.primaryDark}`, mismo texto/tipografía/bordes/padding
- **`button-floating`**: Fondo `{colors.primary}`, texto `{colors.onPrimary}`, tipografía `{typography.bodyLarge}`, bordes `{rounded.special}` (15px), padding `{spacing.md} {spacing.lg}`, sombra alta + overlay rojo oscuro 90%

### Tarjetas
- **`card`**: Fondo `{colors.surface}`, texto `{colors.onSurface}`, tipografía `{typography.bodyMedium}`, bordes `{rounded.none}`, padding `{spacing.md}`, sin sombra (flat)
- **`card-hover`**: Igual que `card` pero con sombra sutil (`0 2px 4px rgba(0,0,0,0.12)`)

### Campo de entrada
- **`input`**: Fondo `{colors.surface}`, texto `{colors.onSurface}`, tipografía `{typography.bodyMedium}`, bordes `{rounded.none}`, padding `{spacing.sm} {spacing.md}`, placeholder `rgba(0,0,0,0.38)`, sin sombra

### Modales y superposiciones
- **`modal`**: Fondo `{colors.surface}`, bordes `{rounded.subtle}` (8px), padding `{spacing.lg}`, sombra media
- **`popover`**: Fondo `{colors.surface}`, bordes `{rounded.subtle}`, padding `{spacing.md}`, sombra media
- **`dropdown`**: Fondo `{colors.surface}`, bordes `{rounded.subtle}`, padding `{spacing.md}`, sombra alta exclusiva
- **`toast`**: Fondo `{colors.neutralDark}`, texto `{colors.neutralLight}`, bordes `{rounded.subtle}`, padding `{spacing.md} {spacing.lg}`, sombra alta exclusiva

### Enlaces y navegación
- **`link`**: Fondo `{colors.surface}`, texto `{colors.primary}`, tipografía `{typography.link}` (10px, Times New Roman, subrayado), hover `{colors.primaryDark}`
- **`navigation`**: Fondo `{colors.surface}`, texto `{colors.onSurface}`, tipografía `{typography.bodyMedium}`, bordes 1px `{colors.border}`, sin sombra
- **`divider`**: Color `{colors.border}`, grosor 1px

---

## Do's and Don'ts

### ✅ Permitido (Do's)
- Usar **Olana exclusivamente** para títulos principales (40px, 45px o 32px móvil)
- Mantener **estética plana** en tarjetas en reposo, campos de entrada y elementos de navegación
- Emplear **blanco (#FFFFFF)** para garantizar contraste adecuado sobre fondos u elementos oscuros
- Usar **múltiplos de 8px** (`spacing.*`) para todos los márgenes y paddings
- Aplicar elevaciones **solo en estados interactivos** (hover, focus) o componentes superpuestos (modales, dropdowns, toasts)
- Usar **Moranga solo para subtítulos** a 25px
- Usar **Times New Roman solo para enlaces** a 10px con subrayado
- Alinear texto a la **izquierda** sin justificar

### ❌ No permitido (Don'ts)
- **Tipografías:** Aplicar opacidad o transparencia en el texto
- **Profundidad:** Aplicar sombras en elementos en reposo
- **Profundidad:** Saturar la interfaz con elevaciones innecesarias
- **Jerarquía tipográfica:** Usar Moranga para cuerpo de texto ni títulos principales
- **Jerarquía tipográfica:** Usar Olana fuera de títulos principales
- **Jerarquía tipográfica:** Usar Times New Roman fuera de enlaces
- **Espaciado:** Usar valores que no sean múltiplos de 8px
- **Formas:** Mezclar redondeos inconsistentes en un mismo componente
- **Color:** Usar colores fuera de la paleta definida sin justificación documentada

---

## Responsive Behavior

### Móvil (< 768px)
- Navegación y contenido en **una sola columna**
- Títulos principales: **32px** (`typography.displayMobile`) conservando **Olana**
- Márgenes exteriores: **24px** (`spacing.marginMobile`)
- Gutters: **16px** (`spacing.gutterMobile`)
- Elevaciones sutiles activadas en **hover/foco** para señalar interactividad

### Tablet (768px - 1023px)
- Transición progresiva de márgenes y gutters
- Retícula de 2-4 columnas según contenido

### Escritorio (≥ 1024px)
- Distribución en **retícula adaptativa** de varias columnas
- Márgenes exteriores: **64px** (`spacing.marginDesktop`)
- Gutters: **24px** (`spacing.gutterDesktop`)
- Títulos principales: **40px/45px** (Olana)
- Interacciones hover completas

---

> **Notas de revisión (REVIEW):**
> 1. `typography.displayLarge.fontFamily` (Olana) — confirmar disponibilidad y licencia
> 2. `typography.subtitle.fontFamily` (Moranga) — confirmar disponibilidad y licencia
> 3. `components.button-floating` overlay — confirmar rojo oscuro 90% opacidad exacta
> 4. `iconography` — no definido en tokens; confirmar si se necesita
> 5. `motion` — no definido en tokens; confirmar curvas/duraciones si hay especificación de animaciones