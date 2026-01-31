# scapeT Landing Page

Landing page informativa para **scapeT**, desarrollada durante la Hackathon de Cursor en El Salvador.

## 🚀 Sobre scapeT

scapeT es una aplicación que te ayuda a planificar tu viaje perfecto. Simplemente ingresa el lugar donde quieres viajar, responde algunas preguntas sobre tus preferencias, y obtén recomendaciones detalladas sobre lugares para visitar, presupuesto estimado y más.

## ✨ Características

- **Diseño Moderno**: Interfaz oscura y profesional inspirada en diseños industriales modernos
- **Animaciones Suaves**: Efectos de fade-in y transiciones fluidas
- **Totalmente Responsive**: Se adapta perfectamente a dispositivos móviles, tablets y desktop
- **Optimizado para Rendimiento**: Carga rápida con Tailwind CSS desde CDN
- **Compatible con GitHub Pages**: Listo para desplegar sin configuración adicional
- **PWA Ready**: Incluye manifest.json y service worker para funcionalidad offline

## 📁 Estructura del Proyecto

```
scapeT-landing/
├── index.html          # Página principal (todo en un archivo)
├── manifest.json        # Configuración PWA
├── sw.js               # Service Worker para PWA
├── .nojekyll           # Configuración GitHub Pages
├── PLAN_TEMPLATE.md    # Plan y prompt para templates
└── README.md          # Este archivo
```

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **Tailwind CSS**: Framework CSS utility-first desde CDN
- **JavaScript (Vanilla)**: Código ligero inline
- **Lucide Icons**: Iconos SVG modernos desde CDN
- **Google Fonts**: Inter y Space Grotesk

## 🎨 Diseño

- **Estilo**: Oscuro, industrial, profesional
- **Color Principal**: #56A87E (verde)
- **Fondo**: Patrón tipo "silk" animado en hero section
- **Tipografía**: Inter (texto), Space Grotesk (títulos técnicos)

## 🚀 Deployment en GitHub Pages

### Opción 1: Desde la Interfaz de GitHub

1. Haz push de todos los archivos a tu repositorio de GitHub
2. Ve a **Settings** > **Pages** en tu repositorio
3. En **Source**, selecciona la rama `main` (o `master`)
4. Selecciona la carpeta `/ (root)`
5. Haz clic en **Save**
6. Tu sitio estará disponible en `https://tu-usuario.github.io/scapeT-landing/`

### Opción 2: Usando GitHub CLI

```bash
# Asegúrate de estar en la rama main
git checkout main

# Haz push de los cambios
git add .
git commit -m "Initial commit: scapeT landing page"
git push origin main
```

Luego sigue los pasos de la Opción 1 para configurar GitHub Pages.

## 📝 Personalización

### Cambiar la URL del Botón CTA

Edita el archivo `index.html` y busca el script al final. Cambia la variable `officialUrl`:

```javascript
const officialUrl = 'https://tu-pagina-oficial.com';
```

### Cambiar la Foto del Equipo

Reemplaza la imagen placeholder en `index.html` (busca la sección "Team Section"):

```html
<img src="ruta/a/tu/imagen.jpg" 
     alt="Equipo de scapeT trabajando" 
     class="w-full h-auto object-cover relative z-10"
     loading="lazy">
```

### Personalizar Colores

Edita las variables CSS en el `<style>` del `index.html`:

```css
:root {
    --primary-green: #56A87E;        /* Color principal */
    --primary-green-dark: #4a9570;   /* Color principal oscuro */
    --primary-green-light: #6bb894;  /* Color principal claro */
}
```

Luego reemplaza todas las clases de Tailwind que usen `text-[#56A87E]` o `bg-[#56A87E]` con el nuevo color.

## 🎨 Secciones de la Landing Page

1. **Hero Section**: Título principal con fondo tipo "silk" verde, descripción y CTAs
2. **Características**: 4 cards explicando qué hace scapeT
3. **Cómo Funciona**: 4 pasos numerados del proceso
4. **Equipo**: Foto del equipo y descripción del proyecto
5. **CTA Final**: Botón de redirección a la página oficial
6. **Footer**: Información del proyecto y links

## ⚡ Optimizaciones Implementadas

- ✅ Tailwind CSS desde CDN (caché del navegador)
- ✅ Lazy loading de imágenes
- ✅ CSS inline crítico optimizado
- ✅ JavaScript mínimo inline
- ✅ Sin dependencias pesadas
- ✅ PWA compatible (manifest.json y service worker)
- ✅ Meta tags Open Graph para redes sociales
- ✅ Rutas relativas para GitHub Pages

## 📱 Compatibilidad

- ✅ Chrome/Edge (últimas versiones)
- ✅ Firefox (últimas versiones)
- ✅ Safari (últimas versiones)
- ✅ Dispositivos móviles (iOS y Android)

## 🎯 Características del Diseño

- **Fondo Oscuro**: Estilo industrial moderno (#020408)
- **Efectos Visuales**: Grid técnico, noise overlay, efectos silk
- **Animaciones**: Fade-up suaves al cargar
- **Hover Effects**: Transiciones en cards y botones
- **Responsive**: Mobile-first con Tailwind CSS

## 🤝 Contribuciones

Este proyecto fue desarrollado durante la Hackathon de Cursor en El Salvador. Para contribuciones o sugerencias, por favor abre un issue en el repositorio.

## 📄 Licencia

Este proyecto fue desarrollado para la Hackathon de Cursor en El Salvador.

---

**Desarrollado con ❤️ durante la Hackathon de Cursor El Salvador**
