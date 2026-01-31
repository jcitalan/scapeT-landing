# 🚀 Guía de Despliegue a GitHub Pages

## Pasos para Publicar tu Landing Page

### 1. Preparar el Repositorio Local

```bash
# Asegúrate de estar en la raíz del proyecto
cd /Users/josuecitalan/Documents/Code/hackaton/scapeT-landing

# Verifica que tienes todos los archivos necesarios
ls -la
```

### 2. Inicializar Git (si aún no lo has hecho)

```bash
# Si es la primera vez
git init
git add .
git commit -m "Initial commit: scapeT landing page"
```

### 3. Crear el Repositorio en GitHub

1. Ve a [https://github.com/new](https://github.com/new)
2. **Nombre del repositorio**: `scapeT-landing` (o el que prefieras)
3. **Descripción**: "Landing page for scapeT - Cursor Hackathon El Salvador"
4. Elige **Público** o **Privado**
5. **NO marques** "Initialize with README" (ya tienes archivos)
6. Haz clic en **"Create repository"**

### 4. Conectar y Subir el Código

```bash
# Agrega el repositorio remoto (reemplaza TU_USUARIO con tu usuario de GitHub)
git remote add origin https://github.com/TU_USUARIO/scapeT-landing.git

# Cambia a la rama main
git branch -M main

# Sube el código
git push -u origin main
```

### 5. Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings** (en la barra superior del repo)
3. En el menú lateral izquierdo, busca y haz clic en **Pages**
4. En la sección **"Source"**:
   - **Branch**: Selecciona `main`
   - **Folder**: Selecciona `/ (root)`
5. Haz clic en **Save**

### 6. Esperar el Despliegue

- GitHub procesará tu sitio (1-2 minutos)
- Verás un mensaje verde: **"Your site is live at..."**
- Tu URL será: `https://TU_USUARIO.github.io/scapeT-landing/`

### 7. Verificar que Todo Funciona

- ✅ Abre la URL en el navegador
- ✅ Verifica que las imágenes se cargan (`./images/team-*.jpeg`)
- ✅ Prueba el calculador de TriPoints
- ✅ Prueba el modal de las fotos del equipo
- ✅ Verifica el modo claro/oscuro
- ✅ Verifica que el logo de Cursor aparece en el footer

## 📝 Actualizaciones Futuras

Después de hacer cambios, simplemente:

```bash
git add .
git commit -m "Descripción de los cambios"
git push origin main
```

GitHub Pages se actualiza automáticamente (puede tardar 1-2 minutos).

## ⚠️ Notas Importantes

1. **Archivo `.nojekyll`**: Ya está creado - evita que GitHub procese el sitio con Jekyll
2. **Rutas relativas**: Las rutas como `./images/team-1.jpeg` funcionan correctamente en GitHub Pages
3. **Assets de Cursor**: Los logos están en `cursor-brand-assets/` y se cargan correctamente

## 🐛 Solución de Problemas

### Las imágenes no cargan
- Verifica que la carpeta `images/` esté en la raíz
- Verifica que los archivos estén en el repositorio

### El sitio no se actualiza
- Espera 1-2 minutos
- Revisa la pestaña **"Actions"** en GitHub para ver el estado del despliegue

### Errores 404
- Verifica que `index.html` esté en la raíz del repositorio
- Verifica que el archivo `.nojekyll` exista

## ✅ Checklist Pre-Despliegue

- [ ] Todos los archivos están en el repositorio
- [ ] Las imágenes del equipo están en `images/`
- [ ] El archivo `.nojekyll` existe
- [ ] El logo de Cursor está en `cursor-brand-assets/`
- [ ] No hay `console.log` en el código (ya limpiado)
- [ ] Todas las rutas son relativas (`./`)

---

**¡Listo para desplegar! 🎉**
