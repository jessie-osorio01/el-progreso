# Subir el proyecto a GitHub y publicarlo (paso a paso)

Reemplaza `TU-USUARIO` por tu usuario de GitHub. Ejecuta los comandos dentro de la carpeta `el-progreso`.

## 1. Crear el repositorio vacío
En https://github.com/new crea el repositorio `el-progreso` (público, **sin** README ni .gitignore).

## 2. Inicializar Git y hacer commits pequeños
```bash
git init -b main
git config user.name "Tu Nombre"
git config user.email "tu-correo@ejemplo.com"

git add README.md
git commit -m "docs: agrega README con descripcion del emprendimiento"

git add docs/PROMPTS.md
git commit -m "docs: documenta prompts, imagenes con IA y moodboard"

git add index.html
git commit -m "feat: agrega pagina web con catalogo, carrito y pedido por WhatsApp"

git add docs/FIREBASE.md docs/GITHUB.md
git commit -m "docs: guia para conectar Firebase y publicar en GitHub"

# cuando tengas las imagenes generadas con IA:
git add img/
git commit -m "feat: agrega logo e imagenes generadas con IA"
```

## 3. Conectar y subir
```bash
git remote add origin https://github.com/TU-USUARIO/el-progreso.git
git push -u origin main
```

## 4. Publicar con GitHub Pages
1. Repositorio → **Settings** → **Pages**.
2. En *Build and deployment* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. Guarda. En 1–2 minutos queda en `https://TU-USUARIO.github.io/el-progreso/`.

## 5. Siguientes cambios
```bash
git add .
git commit -m "fix: ajusta precios del catalogo"
git push
```
Cada commit con mensaje claro suma al criterio de *Git y GitHub* (historial de commits).
