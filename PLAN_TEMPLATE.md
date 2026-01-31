# Plan y Prompt para Adaptar Template a scapeT

## 📋 Información del Proyecto

### Sobre scapeT
- **Nombre**: scapeT
- **Propósito**: Aplicación web que ayuda a planificar viajes perfectos
- **Funcionalidad**: Los usuarios ingresan un destino, responden preguntas sobre preferencias, y reciben recomendaciones detalladas (lugares, presupuesto, actividades)
- **Contexto**: Proyecto desarrollado para Hackathon de Cursor en El Salvador

### Características Clave
- Landing page informativa
- Sección de características (4 cards)
- Sección "Cómo Funciona" (4 pasos)
- Sección del equipo con foto
- Botón CTA que redirige a página oficial
- Diseño responsive y optimizado para GitHub Pages

### Especificaciones Técnicas
- **Color Principal**: #56A87E (verde)
- **Tipografía**: Inter (texto), puede usar Poppins para títulos
- **Estilo**: Limpio, profesional, inspirado en Aura.build
- **Animaciones**: GSAP y anime.js (desde CDN)
- **Iconos**: Lucide Icons
- **PWA**: Compatible con manifest.json y service worker
- **Deployment**: GitHub Pages (sin build process)

---

## 🎯 PROMPT PARA ADAPTAR TEMPLATE

```
Necesito adaptar una plantilla HTML/CSS/JS para crear una landing page profesional 
para "scapeT", una aplicación de planificación de viajes.

REQUISITOS DEL PROYECTO:

1. INFORMACIÓN DEL PRODUCTO:
   - Nombre: scapeT
   - Descripción: Aplicación que ayuda a planificar viajes perfectos ingresando 
     un destino y respondiendo preguntas para obtener recomendaciones personalizadas
   - Contexto: Hackathon de Cursor El Salvador

2. SECCIONES REQUERIDAS:
   a) Hero Section:
      - Título: "Planifica tu Viaje Perfecto"
      - Subtítulo: "scapeT te ayuda a descubrir destinos increíbles y crear el 
        itinerario ideal para tu próxima aventura"
      - Botón CTA: "Descubre cómo funciona" (scroll a características)
      - Fondo: Patrón tipo "silk" con color #56A87E

   b) Características (4 cards):
      - Card 1: "Ingresa tu Destino" - Icono de ubicación
      - Card 2: "Responde Preguntas" - Icono de pregunta/info
      - Card 3: "Obtén Recomendaciones" - Icono de estrella/recomendación
      - Card 4: "Planificación Completa" - Icono de check/planificación

   c) Cómo Funciona (4 pasos numerados):
      - Paso 1: "Escribe tu Destino" - Ingresa ciudad o país
      - Paso 2: "Responde las Preguntas" - Comparte gustos y presupuesto
      - Paso 3: "Recibe tu Plan" - Obtén recomendaciones detalladas
      - Paso 4: "¡Viaja y Disfruta!" - Disfruta tu aventura

   d) Equipo:
      - Título: "Nuestro Equipo"
      - Imagen del equipo trabajando (placeholder por ahora)
      - Descripción sobre el equipo y el proyecto

   e) CTA Final:
      - Título: "¿Listo para Planificar tu Próximo Viaje?"
      - Descripción: "Descubre todas las funcionalidades de scapeT..."
      - Botón: "Ir a la Página Oficial" (redirige a URL oficial)

   f) Footer:
      - Copyright: "© 2026 scapeT - Hackathon Cursor El Salvador"
      - Texto adicional: "Hecho con ❤️ por el equipo scapeT"

3. ESPECIFICACIONES DE DISEÑO:
   - Color Principal: #56A87E (verde)
   - Color Secundario: Variaciones del verde (#4a9570, #6bb894)
   - Tipografía: Inter para texto, puede usar Poppins para títulos
   - Estilo: Limpio, profesional, minimalista (inspirado en Aura.build)
   - Animaciones: Suaves, con GSAP y anime.js
   - Responsive: Mobile-first, debe funcionar en todos los dispositivos

4. TECNOLOGÍAS A USAR:
   - HTML5 semántico
   - CSS3 con variables CSS
   - JavaScript vanilla (sin frameworks pesados)
   - GSAP desde CDN: https://cdn.jsdelivr.net/npm/gsap@3.12.5/dist/gsap.min.js
   - ScrollTrigger: https://cdn.jsdelivr.net/npm/gsap@3.12.5/dist/ScrollTrigger.min.js
   - Anime.js: https://cdn.jsdelivr.net/npm/animejs@3.2.1/lib/anime.min.js
   - Lucide Icons: https://unpkg.com/lucide@latest/dist/umd/lucide.js
   - Google Fonts: Inter y Poppins

5. OPTIMIZACIONES REQUERIDAS:
   - Compatible con GitHub Pages (sin build process)
   - Rutas relativas para todos los assets
   - Lazy loading de imágenes
   - Animaciones solo cuando están en viewport
   - PWA compatible (manifest.json y service worker básico)
   - Meta tags Open Graph para redes sociales

6. ELEMENTOS ESPECIALES:
   - Header fijo con efecto glassmorphism sutil
   - Fondo tipo "silk" animado en hero section (color #56A87E)
   - Cards con hover effects sutiles
   - Animaciones de entrada al hacer scroll
   - Botones con microinteracciones

INSTRUCCIONES:
1. Mantén la estructura HTML semántica de la plantilla
2. Adapta los colores al esquema verde (#56A87E)
3. Reemplaza el contenido con la información de scapeT
4. Asegúrate de que todas las secciones requeridas estén presentes
5. Optimiza para GitHub Pages (rutas relativas, sin build)
6. Agrega las librerías desde CDN en el <head>
7. Mantén el diseño responsive y profesional
8. Agrega animaciones sutiles pero no excesivas

ARCHIVOS A CREAR/MODIFICAR:
- index.html (estructura completa)
- styles.css (estilos personalizados)
- script.js (animaciones y lógica)
- manifest.json (PWA)
- sw.js (service worker básico)
- README.md (documentación)

NOTAS IMPORTANTES:
- El sitio debe funcionar completamente estático (sin servidor)
- Todas las animaciones deben tener fallbacks si las librerías no cargan
- El diseño debe ser accesible y semántico
- Optimizado para conexiones lentas
```

---

## ✅ Checklist de Personalización

### Contenido
- [ ] Reemplazar todos los textos con información de scapeT
- [ ] Actualizar títulos y subtítulos
- [ ] Agregar descripciones de características
- [ ] Incluir los 4 pasos de "Cómo Funciona"
- [ ] Agregar información del equipo
- [ ] Configurar botón CTA con URL oficial

### Diseño Visual
- [ ] Cambiar color principal a #56A87E
- [ ] Actualizar tipografía a Inter/Poppins
- [ ] Aplicar fondo tipo "silk" en hero
- [ ] Personalizar iconos (usar Lucide Icons)
- [ ] Ajustar espaciado y layout
- [ ] Verificar responsive design

### Funcionalidad
- [ ] Integrar GSAP y ScrollTrigger
- [ ] Agregar animaciones con anime.js
- [ ] Configurar Lucide Icons
- [ ] Implementar scroll suave
- [ ] Agregar efectos hover
- [ ] Configurar PWA (manifest.json, sw.js)

### Optimización
- [ ] Verificar rutas relativas
- [ ] Agregar lazy loading a imágenes
- [ ] Optimizar animaciones (solo en viewport)
- [ ] Agregar meta tags Open Graph
- [ ] Configurar service worker
- [ ] Probar en GitHub Pages

### Testing
- [ ] Probar en Chrome/Edge
- [ ] Probar en Firefox
- [ ] Probar en Safari
- [ ] Probar en móviles (iOS/Android)
- [ ] Verificar animaciones
- [ ] Verificar responsive
- [ ] Verificar accesibilidad

---

## 📝 Pasos para Usar el Prompt

1. **Elige una plantilla**:
   - Busca en: ThemeForest, HTML5 UP, Colorlib, etc.
   - Preferiblemente HTML/CSS/JS vanilla (sin React/Vue)
   - Que sea responsive y moderna

2. **Copia el prompt completo** y úsalo con:
   - ChatGPT/Claude para adaptar la plantilla
   - O úsalo como guía manual

3. **Reemplaza el contenido**:
   - Usa la información de scapeT proporcionada
   - Mantén la estructura de la plantilla
   - Personaliza colores y estilos

4. **Integra las tecnologías**:
   - Agrega GSAP, anime.js, Lucide desde CDN
   - Configura PWA
   - Optimiza para GitHub Pages

5. **Prueba y ajusta**:
   - Verifica que todo funcione
   - Prueba en diferentes navegadores
   - Optimiza rendimiento

---

## 🎨 Paleta de Colores

```
Primario:     #56A87E (verde principal)
Primario Oscuro: #4a9570
Primario Claro: #6bb894
Texto Oscuro: #0f172a
Texto Medio:  #334155
Texto Claro:  #64748b
Fondo Claro: #f8fafc
Fondo Blanco: #ffffff
```

---

## 📦 Estructura de Archivos Final

```
scapeT-landing/
├── index.html          # Página principal
├── styles.css          # Estilos personalizados
├── script.js           # Animaciones y lógica
├── manifest.json       # PWA manifest
├── sw.js              # Service Worker
├── .nojekyll          # Para GitHub Pages
├── README.md          # Documentación
└── PLAN_TEMPLATE.md   # Este archivo
```

---

## 💡 Tips Adicionales

1. **Si la plantilla usa imágenes**: Reemplázalas con placeholders o imágenes reales del equipo
2. **Si usa frameworks**: Convierte a vanilla JS o mantén solo lo esencial
3. **Si tiene build process**: Extrae solo los archivos finales (HTML/CSS/JS)
4. **Optimización**: Minifica CSS/JS si es necesario, pero mantén legibilidad
5. **GitHub Pages**: Asegúrate de que `index.html` esté en la raíz

---

**¡Listo para usar!** Copia el prompt y úsalo con tu plantilla favorita. 🚀
