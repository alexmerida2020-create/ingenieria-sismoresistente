# 🚀 Guía de Despliegue en GitHub Pages

## Opción 1: Despliegue automático (Recomendado)

### Paso 1: Crear repositorio en GitHub
1. Ve a [GitHub](https://github.com)
2. Haz clic en el botón verde "New" o "New repository"
3. Nombra tu repositorio: `ingenieria-sismoresistente`
4. Selecciona "Public" (para usar GitHub Pages gratis)
5. Marca "Add a README file" (opcional, ya tienes uno)
6. Haz clic en "Create repository"

### Paso 2: Subir archivos al repositorio

#### Opción A: Usando GitHub Web Interface
1. En tu repositorio, haz clic en "Add file" → "Upload files"
2. Arrastra estos archivos:
   - `ingenieria-sismoresistente.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
3. Escribe un mensaje de commit: "Agregar material educativo de ingeniería sismoresistente"
4. Haz clic en "Commit changes"

#### Opción B: Usando Git desde tu terminal
```bash
# 1. Inicializar repositorio local
git init

# 2. Agregar todos los archivos
git add .

# 3. Hacer primer commit
git commit -m "Agregar material educativo de ingeniería sismoresistente"

# 4. Conectar con repositorio remoto
git remote add origin https://github.com/TU-USUARIO/ingenieria-sismoresistente.git

# 5. Renombrar rama a main (si es necesario)
git branch -M main

# 6. Subir archivos
git push -u origin main
```

### Paso 3: Activar GitHub Pages
1. En tu repositorio, ve a **Settings** (Configuración)
2. En el menú lateral, busca **Pages**
3. En "Source", selecciona:
   - Branch: `main`
   - Folder: `/ (root)`
4. Haz clic en **Save**
5. Espera unos segundos y verás un mensaje: "Your site is published at..."

### Paso 4: Renombrar archivo (importante)
Para que GitHub Pages reconozca tu página principal:
1. Renombra `ingenieria-sismoresistente.html` a `index.html`
2. Commit el cambio:
```bash
git mv ingenieria-sismoresistente.html index.html
git commit -m "Renombrar a index.html para GitHub Pages"
git push
```

### Paso 5: Acceder a tu sitio
Tu sitio estará disponible en:
```
https://TU-USUARIO.github.io/ingenieria-sismoresistente/
```

## Opción 2: Despliegue rápido sin Git

### Usando GitHub Desktop (GUI)
1. Descarga [GitHub Desktop](https://desktop.github.com/)
2. Inicia sesión con tu cuenta de GitHub
3. File → New Repository
4. Nombra el repositorio: `ingenieria-sismoresistente`
5. Elige la ubicación local donde tienes los archivos
6. Copia los archivos a esa carpeta
7. En GitHub Desktop:
   - Verás los archivos en "Changes"
   - Escribe un mensaje de commit
   - Haz clic en "Commit to main"
   - Haz clic en "Publish repository"
8. Sigue el Paso 3 de la Opción 1 para activar Pages

## Opción 3: Usando servicios alternativos

### Netlify (Muy fácil, sin necesidad de Git)
1. Ve a [Netlify](https://www.netlify.com/)
2. Regístrate gratis
3. Arrastra y suelta tu archivo HTML en el área de "Drop"
4. Tu sitio estará en línea en segundos con una URL como: `random-name.netlify.app`
5. Puedes personalizar el nombre en Site settings

### Vercel
1. Ve a [Vercel](https://vercel.com/)
2. Regístrate con tu cuenta de GitHub
3. New Project → Import Git Repository
4. Selecciona tu repositorio
5. Deploy

## 🔧 Solución de problemas comunes

### Problema: "404 - Page not found"
**Solución**: Asegúrate de que el archivo se llama `index.html`, no `ingenieria-sismoresistente.html`

### Problema: Los estilos no se cargan
**Solución**: Los estilos están embebidos en el HTML, así que este problema no debería ocurrir. Si ocurre, revisa la consola del navegador (F12).

### Problema: "Permission denied" al hacer push
**Solución**: 
1. Verifica que tu SSH key esté configurada, o
2. Usa HTTPS y proporciona tu token de acceso personal

### Problema: Cambios no se reflejan
**Solución**: 
1. GitHub Pages puede tardar 1-2 minutos en actualizar
2. Limpia la caché del navegador (Ctrl + Shift + R)

## 📱 Compartir tu sitio

Una vez desplegado, puedes compartir la URL:
```
https://tu-usuario.github.io/ingenieria-sismoresistente/
```

### Ideas para compartir:
- En tu CV como proyecto personal
- Con compañeros de clase
- Con profesores como material complementario
- En redes sociales profesionales (LinkedIn)

## 🎓 Personalización

Para personalizar el contenido:
1. Edita `index.html` (antes `ingenieria-sismoresistente.html`)
2. Guarda los cambios
3. Haz commit y push:
```bash
git add index.html
git commit -m "Actualizar contenido"
git push
```

## ✨ Mejoras sugeridas

- Agregar más casos de estudio
- Incluir calculadoras interactivas con JavaScript
- Añadir videos explicativos embebidos
- Crear sección de ejercicios prácticos
- Agregar galería de imágenes de daños sísmicos

---

¿Tienes problemas? Abre un [issue en el repositorio](https://github.com/TU-USUARIO/ingenieria-sismoresistente/issues) y estaré encantado de ayudarte.
