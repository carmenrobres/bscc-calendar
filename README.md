# Mi Notion Personal

Web estática que funciona como Notion: sidebar con páginas, bloques editables (texto, títulos, listas, tablas), y guardado directo en GitHub.

## Archivos

```
index.html   ← toda la aplicación (una sola página)
data.json    ← tu contenido (páginas y bloques)
README.md    ← este archivo
```

## Despliegue en GitHub Pages

1. Sube los tres archivos a un repositorio de GitHub
2. Ve a **Settings → Pages**
3. Source: **Deploy from branch** → `main` → `/root`
4. Guarda. En ~1 minuto tendrás la web en:
   `https://TU-USUARIO.github.io/NOMBRE-REPO`

## Uso

### Ver contenido
Abre la web normalmente. Navega entre páginas con el menú lateral.

### Editar
1. Haz clic en **"Modo edición"** en la parte inferior del sidebar
2. Introduce la contraseña: **IBD1234**
3. Edita directamente: haz clic en cualquier texto para modificarlo
4. Añade bloques con el botón **"＋ Bloque"**
5. Cuando termines, haz clic en **"Guardar en GitHub"**

### Guardar en GitHub
Al guardar necesitarás:
- Tu **nombre de usuario** de GitHub
- El **nombre del repositorio**
- Un **Personal Access Token** (con permiso `repo`)

Puedes marcar "Recordar en este navegador" para no tener que escribirlos cada vez.

## Tipos de bloques disponibles

- **Texto** — párrafos normales
- **H1, H2, H3** — títulos de distintos tamaños
- **Lista** — puntos con viñeta
- **Numerada** — lista numerada
- **Tabla** — con filas y columnas editables

## Contraseña de edición

La contraseña está en el archivo `index.html` (línea con `const PASSWORD`).
Para cambiarla, edita esa línea directamente en el archivo.

## Personalización

Edita `data.json` directamente para cambiar:
- `site.title` — nombre del espacio de trabajo
- `site.icon` — emoji del workspace
- `pages` — array con todas las páginas y sus bloques
