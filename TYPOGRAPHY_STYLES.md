# Sistema de Tipografía y Estilos - scapeT Landing Page

Documentación completa del sistema de tipografía y estilos utilizados en la landing page de scapeT. **Nota: Este documento NO incluye colores, solo tipografía y estilos.**

---

## 📚 Tipografías Utilizadas

### Fuentes Principales

#### 1. **Inter** (Cuerpo de Texto)
- **Fuente**: `'Inter', sans-serif`
- **Pesos disponibles**: 300, 400, 500, 600, 700, 800
- **Uso**: Texto general, párrafos, descripciones, contenido principal
- **Google Fonts URL**: 
  ```
  https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap
  ```

#### 2. **Space Grotesk** (Técnica/Títulos)
- **Fuente**: `'Space Grotesk', monospace`
- **Pesos disponibles**: 400, 500, 600, 700
- **Uso**: Títulos técnicos, navegación, badges, botones, elementos destacados
- **Google Fonts URL**: 
  ```
  https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&display=swap
  ```

### Clase CSS Personalizada

```css
.font-tech {
    font-family: 'Space Grotesk', monospace;
}
```

---

## 📏 Sistema de Tipografía

### Jerarquía de Tamaños

| Clase Tailwind | Tamaño (rem) | Tamaño (px) | Uso |
|----------------|--------------|-------------|-----|
| `text-[10px]` | 0.625rem | 10px | Footer, texto muy pequeño |
| `text-xs` | 0.75rem | 12px | Labels, badges, navegación |
| `text-sm` | 0.875rem | 14px | Texto secundario, descripciones de cards |
| `text-base` | 1rem | 16px | Texto base (no usado explícitamente) |
| `text-lg` | 1.125rem | 18px | Texto destacado |
| `text-xl` | 1.25rem | 20px | Títulos de cards |
| `text-2xl` | 1.5rem | 24px | Subtítulos |
| `text-3xl` | 1.875rem | 30px | Títulos de sección (mobile) |
| `text-4xl` | 2.25rem | 36px | Títulos grandes |
| `text-5xl` | 3rem | 48px | Hero title (mobile) |
| `text-7xl` | 4.5rem | 72px | Hero title (tablet) |
| `text-8xl` | 5rem | 80px | Hero title (desktop) |

### Pesos de Fuente

| Clase | Peso | Uso |
|-------|------|-----|
| `font-light` | 300 | Descripciones suaves, texto secundario |
| `font-normal` | 400 | Texto base (default) |
| `font-medium` | 500 | No usado frecuentemente |
| `font-semibold` | 600 | Títulos principales, headings |
| `font-bold` | 700 | Números destacados, badges importantes |
| `font-extrabold` | 800 | No usado frecuentemente |

### Letter Spacing (Tracking)

| Clase | Valor | Uso |
|-------|-------|-----|
| `tracking-tighter` | -0.05em | Hero titles grandes |
| `tracking-tight` | -0.025em | Títulos de sección |
| `tracking-normal` | 0em | Texto normal |
| `tracking-wide` | 0.025em | No usado |
| `tracking-widest` | 0.1em | Navegación, botones, labels |
| `tracking-[0.2em]` | 0.2em | Logo, status indicators |
| `tracking-[0.3em]` | 0.3em | Section labels |

### Text Transform

| Clase | Transformación | Uso |
|-------|----------------|-----|
| `uppercase` | MAYÚSCULAS | Navegación, botones, títulos técnicos |
| `lowercase` | minúsculas | No usado |
| `capitalize` | Primera Letra | No usado |
| `normal-case` | Normal | Texto general |

### Line Height (Leading)

| Clase | Valor | Uso |
|-------|-------|-----|
| `leading-[0.9]` | 0.9 | Hero titles - Muy compacto |
| `leading-tight` | 1.25 | Títulos |
| `leading-normal` | 1.5 | Texto normal |
| `leading-relaxed` | 1.625 | Párrafos largos |
| `leading-loose` | 2 | No usado frecuentemente |

---

## 🎨 Estilos de Texto Específicos

### Hero Section

#### Título Principal
```css
font-semibold
text-5xl md:text-7xl lg:text-8xl
tracking-tighter
uppercase
leading-[0.9]
text-glow
```

#### Descripción Hero
```css
font-light
text-lg md:text-xl
leading-relaxed
border-l (borde izquierdo decorativo)
pl-6 (padding izquierdo)
```

### Navegación

```css
font-tech
text-xs
tracking-widest
uppercase
```

### Section Headers

#### Label (pequeño arriba del título)
```css
font-tech
text-xs
tracking-[0.3em]
uppercase
```

#### Título de Sección
```css
font-semibold
text-3xl md:text-5xl
tracking-tight
uppercase
```

### Cards / Features

#### Título de Card
```css
font-semibold
text-xl
tracking-tight
uppercase
```

#### Descripción de Card
```css
font-light (o normal)
text-sm
leading-relaxed (o normal)
```

### Botones

```css
font-tech
uppercase
tracking-widest
text-sm (o text-xs)
```

### Badges / Labels Pequeños

```css
font-tech
text-xs
tracking-widest
uppercase
```

---

## ✨ Efectos de Texto

### Text Glow (Sombra Sutil)

```css
.text-glow {
    text-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
}

.dark .text-glow {
    text-shadow: 0 0 20px rgba(255, 255, 255, 0.1);
}
```

### Antialiasing

```css
antialiased  /* Clase aplicada al body para suavizar texto */
```

---

## 📐 Espaciado y Estructura

### Padding/Margin Típicos

| Clase | Valor | Uso |
|-------|-------|-----|
| `py-32` | 8rem (128px) | Secciones principales |
| `py-40` | 10rem (160px) | Hero, Team sections |
| `p-8` | 2rem (32px) | Padding interno de cards |
| `mb-2` | 0.5rem (8px) | Entre título y texto |
| `mb-4` | 1rem (16px) | Espaciado medio |
| `mb-6` | 1.5rem (24px) | Espaciado grande |
| `mb-8` | 2rem (32px) | Espaciado muy grande |
| `mb-10` | 2.5rem (40px) | Espaciado extra |
| `mb-16` | 4rem (64px) | Espaciado entre secciones |
| `mb-20` | 5rem (80px) | Espaciado máximo |

### Max Width Containers

| Clase | Valor | Uso |
|-------|-------|-----|
| `max-w-xl` | 36rem (576px) | Texto descriptivo |
| `max-w-2xl` | 42rem (672px) | Contenido medio |
| `max-w-5xl` | 64rem (1024px) | Secciones principales |
| `max-w-6xl` | 72rem (1152px) | Galerías |
| `max-w-7xl` | 80rem (1280px) | Contenedor principal |

---

## 💻 Código de Implementación

### Importación de Fuentes

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
```

### CSS Base

```css
/* Body base */
body {
    font-family: 'Inter', sans-serif;
    font-weight: 400;
    line-height: 1.5;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

/* Fuente técnica */
.font-tech {
    font-family: 'Space Grotesk', monospace;
}
```

### Variables CSS (Sistema de Tokens)

```css
:root {
    /* Tamaños de texto */
    --text-xs: 0.75rem;      /* 12px */
    --text-sm: 0.875rem;    /* 14px */
    --text-base: 1rem;      /* 16px */
    --text-lg: 1.125rem;    /* 18px */
    --text-xl: 1.25rem;     /* 20px */
    --text-2xl: 1.5rem;    /* 24px */
    --text-3xl: 1.875rem;  /* 30px */
    --text-4xl: 2.25rem;   /* 36px */
    --text-5xl: 3rem;      /* 48px */
    --text-7xl: 4.5rem;    /* 72px */
    --text-8xl: 5rem;      /* 80px */
    
    /* Letter spacing */
    --tracking-tighter: -0.05em;
    --tracking-tight: -0.025em;
    --tracking-normal: 0em;
    --tracking-wide: 0.025em;
    --tracking-widest: 0.1em;
    --tracking-extra: 0.2em;
    --tracking-ultra: 0.3em;
    
    /* Line height */
    --leading-none: 1;
    --leading-tight: 1.25;
    --leading-snug: 1.375;
    --leading-normal: 1.5;
    --leading-relaxed: 1.625;
    --leading-loose: 2;
    
    /* Font weights */
    --font-light: 300;
    --font-normal: 400;
    --font-medium: 500;
    --font-semibold: 600;
    --font-bold: 700;
    --font-extrabold: 800;
}
```

---

## 📋 Ejemplos de Uso

### Hero Title
```html
<h1 class="text-5xl md:text-7xl lg:text-8xl font-semibold tracking-tighter uppercase leading-[0.9] text-glow">
    Plan Your Perfect Trip
</h1>
```

### Section Header
```html
<span class="font-tech text-xs tracking-[0.3em] uppercase">Features</span>
<h2 class="text-3xl md:text-5xl font-semibold tracking-tight uppercase">
    What Does scapeT Do?
</h2>
```

### Card Title
```html
<h3 class="text-xl font-semibold tracking-tight uppercase">
    Enter Your Destination
</h3>
```

### Navigation Link
```html
<a href="#" class="font-tech text-xs tracking-widest uppercase">
    Features
</a>
```

### Button
```html
<button class="font-tech uppercase tracking-widest text-sm">
    Get Started
</button>
```

### Description Text
```html
<p class="text-sm font-light leading-relaxed">
    Simply type the place where you want to travel...
</p>
```

---

## 🎯 Reglas de Diseño

1. **Inter** se usa para todo el texto general y legible
2. **Space Grotesk** se usa para elementos técnicos, navegación y elementos que necesitan destacar
3. Los títulos principales siempre usan `uppercase` y `tracking-tight` o `tracking-tighter`
4. La navegación y botones siempre usan `font-tech`, `uppercase` y `tracking-widest`
5. Los textos largos usan `leading-relaxed` para mejor legibilidad
6. Los hero titles usan `leading-[0.9]` para un look más compacto y moderno
7. Los labels pequeños siempre usan `text-xs` con `tracking-widest` o `tracking-[0.3em]`

---

## 📝 Notas Importantes

- **No se incluyen colores** en este documento - solo tipografía y estilos
- Todas las medidas son responsivas usando breakpoints de Tailwind (`md:`, `lg:`)
- El sistema está optimizado para legibilidad y jerarquía visual clara
- Las fuentes se cargan desde Google Fonts para mejor rendimiento
- El antialiasing está habilitado para suavizar el texto en todos los navegadores

---

**Documento generado para implementación en el frontend del SaaS scapeT**
