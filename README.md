# Mi Caja - Ventas y ganancias

App web para un vendedor: registra ventas, calcula la ganancia del mes, proyecta el cierre,
compara lo estimado con lo real y reconoce productos con una foto. Funciona sin conexión
y se puede instalar en el celular como una app.

## Qué incluye

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app completa (un solo archivo, sin dependencias) |
| `manifest.webmanifest` | Datos de instalación (nombre, colores, íconos) |
| `sw.js` | Hace que funcione sin conexión |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | Íconos de la app |
| `.nojekyll` | Evita que GitHub Pages procese los archivos |

## Publicarla gratis con GitHub Pages

1. Creá una cuenta en https://github.com (si no tenés) y tocá **New repository**.
   Ponele un nombre, por ejemplo `mi-caja`, dejalo en **Public** y creá el repositorio.
2. Tocá **uploading an existing file** y subí **todos** los archivos de esta carpeta
   (incluido `.nojekyll`). Confirmá con **Commit changes**.
3. Entrá a **Settings > Pages**. En *Build and deployment* elegí
   **Deploy from a branch**, rama **main**, carpeta **/ (root)** y guardá.
4. Esperá uno o dos minutos. La app queda en:
   `https://TU-USUARIO.github.io/mi-caja/`

## Instalarla en el celular

- **Android (Chrome):** abrí el link, menú de los tres puntos > **Instalar app** (o *Agregar a pantalla de inicio*).
- **iPhone (Safari):** botón Compartir > **Agregar a pantalla de inicio**.

## Convertirla en APK

1. Entrá a https://www.pwabuilder.com y pegá el link de GitHub Pages.
2. Elegí **Package for stores > Android** y descargá el paquete.
3. Instalá el APK en el celular (habilitando instalar apps de fuentes desconocidas).
   Para publicarla en Play Store hay que firmar el paquete con tu propia clave.

## Datos importantes

- **Los datos se guardan en el dispositivo y por dirección web.** Si cambiás de link o de celular,
  no se pasan solos: usá **Ajustes > Exportar copia** en el viejo e **Importar copia** en el nuevo.
- Hacé una copia de seguridad de vez en cuando.
- Fuera de Claude no está el botón "Que Claude identifique el producto". El reconocimiento por
  foto funciona igual con el método propio de la app (color, diseño y bordes).
- Cuando modifiques `index.html`, subí el número de `VERSION` en `sw.js` (por ejemplo `v2`)
  para que los celulares descarguen la versión nueva.
- Sacá 2 o 3 fotos de cada producto desde distintos ángulos y con buena luz; mejora mucho el reconocimiento.
