# 📄 Visor de PDF con GitHub Pages

Este proyecto te permite publicar un PDF en línea de forma gratuita usando GitHub Pages.

## 🚀 Pasos para publicar

### 1. Preparar los archivos
- ✅ Ya tienes el archivo `index.html`
- 📌 **Importante:** Coloca tu archivo PDF en esta carpeta y nómbralo `documento.pdf`
  - O edita `index.html` (línea 42) para cambiar el nombre del PDF

### 2. Crear cuenta en GitHub
1. Ve a [GitHub.com](https://github.com)
2. Haz clic en "Sign up" (Registrarse)
3. Crea tu cuenta gratuita

### 3. Crear repositorio
1. Una vez dentro de GitHub, haz clic en el botón verde "New" (Nuevo)
2. Nombre del repositorio: `pdf-viewer` (o el nombre que prefieras)
3. Selecciona "Public" (Público)
4. **NO** marques "Add a README file"
5. Haz clic en "Create repository"

### 4. Subir archivos
Tienes dos opciones:

#### Opción A: Subir desde la web (Más fácil)
1. En la página de tu repositorio, haz clic en "uploading an existing file"
2. Arrastra estos archivos:
   - `index.html`
   - `documento.pdf` (tu archivo PDF)
3. Escribe un mensaje como "Subir archivos iniciales"
4. Haz clic en "Commit changes"

#### Opción B: Usar Git (Avanzado)
```bash
git init
git add .
git commit -m "Primer commit"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/pdf-viewer.git
git push -u origin main
```

### 5. Activar GitHub Pages
1. Ve a tu repositorio en GitHub
2. Haz clic en "Settings" (Configuración)
3. En el menú izquierdo, haz clic en "Pages"
4. En "Source" (Fuente), selecciona "main" branch
5. Haz clic en "Save"
6. ⏳ Espera 1-2 minutos

### 6. Obtener tu enlace
Tu sitio estará disponible en:
```
https://TU-USUARIO.github.io/pdf-viewer
```

Reemplaza `TU-USUARIO` con tu nombre de usuario de GitHub.

### 7. Crear código QR
1. Ve a [QR Code Generator](https://www.qr-code-generator.com/)
2. Pega tu enlace de GitHub Pages
3. Descarga el código QR
4. ¡Listo! Ya puedes compartir el QR

## ⚙️ Personalización

### Cambiar el PDF mostrado
Edita la línea 42 en `index.html`:
```html
<iframe class="pdf-viewer" src="./documento.pdf#page=1">
```

### Mostrar una página específica
Cambia `#page=1` por el número de página:
```html
<iframe class="pdf-viewer" src="./documento.pdf#page=15">
```

### Cambiar el título
Edita las líneas 6 y 37 en `index.html`:
```html
<title>Mi Documento PDF</title>
...
<h1>Mi Documento PDF</h1>
```

## 📱 Características
- ✅ 100% Gratuito
- ✅ Responsive (se adapta a móviles)
- ✅ Sin límite de tiempo
- ✅ Fácil de actualizar
- ✅ Soporte para cualquier PDF

## 🔄 Actualizar el PDF
1. Ve a tu repositorio en GitHub
2. Haz clic en el archivo PDF
3. Haz clic en el icono de lápiz o "Delete this file"
4. Sube el nuevo PDF con el mismo nombre
5. Haz commit
6. En 1-2 minutos se actualizará automáticamente

## 🆘 Solución de problemas

### El PDF no se muestra
- Verifica que el nombre del archivo en `index.html` coincida con el nombre del PDF
- Asegúrate de que el PDF esté en la misma carpeta que `index.html`
- Algunos navegadores móviles no muestran PDFs en iframes (ofrecen descarga)

### GitHub Pages no aparece en Settings
- Asegúrate de que el repositorio sea público
- Espera unos minutos después de crear el repositorio

### El enlace da error 404
- Espera 2-3 minutos después de activar GitHub Pages
- Verifica que el archivo se llame exactamente `index.html` (minúsculas)

## 📞 Recursos adicionales
- [Documentación de GitHub Pages](https://docs.github.com/es/pages)
- [Tutorial de Git en español](https://git-scm.com/book/es/v2)

---

**¡Éxito con tu proyecto!** 🎉
