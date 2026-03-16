# BSC — Eventos & Funding Calls

## Setup (una sola vez)

### 1. Sube los archivos al repo
Asegúrate de tener en el repo:
- `index.html`
- `data.json`  
- `.github/workflows/update-data.yml`

### 2. Crea el GitHub Secret
Ve a: **Settings → Secrets and variables → Actions → New repository secret**

- Nombre: `DATA_TOKEN`
- Valor: tu Personal Access Token con permiso `repo`

### 3. Activa GitHub Pages
**Settings → Pages → Source: main → / (root)**

---

## Uso diario

1. Abre la web
2. Haz clic en **"Editar contenido"** (sidebar inferior)
3. Contraseña: `IBD1234`
4. Edita lo que necesites
5. Clic en **"Guardar"** → los datos se publican automáticamente

### Primera vez guardando desde un navegador nuevo
La primera vez que guardes desde un ordenador nuevo, el sistema pedirá tu Personal Access Token. Se guarda en el navegador (localStorage) y no vuelve a pedirlo.

---

## Arquitectura de seguridad

- **Contraseña de edición** (`IBD1234`): solo en el navegador, protege la UI
- **Token de GitHub**: guardado en GitHub Secrets (nunca visible en el código)
- **GitHub Actions**: recibe los datos y hace el commit en el servidor
- Nadie puede ver el token aunque inspeccione el código fuente
