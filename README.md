# Portal de Operaciones Compas

Dashboard de inventario y OTIF desplegado en GitHub Pages.

## Estructura del repositorio

```
Portal-de-operaciones-Compas/
├── index.html       ← Dashboard principal (renombrar desde dashboard_inventario.html)
├── datos.xlsx       ← Archivo Excel con los datos (actualizar periódicamente)
└── README.md
```

## Cómo actualizar los datos

1. Abre tu repositorio en GitHub: https://github.com/ftrevinor001-tr/Portal-de-operaciones-Compas
2. Haz clic en el archivo `datos.xlsx`
3. Haz clic en el ícono del lápiz (editar) → **"Upload files"**
4. Sube tu nuevo Excel con el mismo nombre `datos.xlsx`
5. Haz clic en **"Commit changes"**
6. En ~1 minuto, al abrir el dashboard se cargará la información nueva automáticamente

## Configuración del auto-carga

En el archivo `index.html`, al inicio del bloque `<script>` hay dos variables:

```javascript
const AUTO_LOAD_FILE = 'datos.xlsx';  // Nombre del Excel en el repositorio
const AUTO_LOAD_ENABLED = true;       // false = siempre mostrar pantalla de carga manual
```

Cambia `AUTO_LOAD_FILE` si usas un nombre diferente para tu Excel.

## Primer despliegue

1. Descarga `dashboard_inventario.html` y renómbralo a `index.html`
2. Sube tanto `index.html` como `datos.xlsx` a la raíz del repositorio
3. En GitHub → Settings → Pages → Source: **"Deploy from branch"** → branch: **main** → folder: **/ (root)**
4. Guarda. En ~2 minutos el sitio estará disponible en:
   https://ftrevinor001-tr.github.io/Portal-de-operaciones-Compas/
