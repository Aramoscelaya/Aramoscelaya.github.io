# aramoscelaya.github.io

Portafolio personal — Alejandro Ramos, Desarrollador de Software.

## Estructura

```
aramoscelaya.github.io/
├── index.html              # Página principal
├── README.md               # Este archivo
└── assets/
    ├── screenshots/        # Capturas de pantalla de proyectos
    │   └── amipattern.png  # Preview de AmiPattern (1200×630 px recomendado)
    └── favicon/            # Íconos del sitio
        ├── favicon.ico
        ├── favicon-32x32.png
        └── apple-touch-icon.png
```

## Cómo agregar un proyecto nuevo

1. Tomar screenshot del proyecto (1200×630 px o similar 2:1)
2. Guardarla en `assets/screenshots/nombre-proyecto.png`
3. Duplicar el bloque comentado en `index.html` dentro de `.projects-grid`
4. Descomentar y llenar: `href`, título, descripción, tags, status y la ruta de la imagen

```html
<a href="https://github.com/Aramoscelaya/REPO" class="project-card" target="_blank" rel="noopener">
  <div class="project-preview">
    <img src="assets/screenshots/nombre-proyecto.png" alt="Vista previa de Nombre" />
  </div>
  <p class="project-title">Nombre del proyecto</p>
  <p class="project-desc">Descripción breve.</p>
  <div class="project-tags">
    <span class="tag">PHP</span>
    <span class="tag">MySQL</span>
  </div>
  <div class="project-footer">
    <span class="project-status">Producción</span>
    <span class="link-pill">ver en GitHub <i class="ti ti-arrow-up-right"></i></span>
  </div>
</a>
```

## Deploy

El sitio se publica automáticamente en `aramoscelaya.github.io` al hacer push a `main`.

```bash
git add .
git commit -m "feat: agregar proyecto X"
git push origin main
```
