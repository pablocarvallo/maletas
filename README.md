# Maletas

App web para iPhone que organiza lo que guardas en tus maletas: mantas (quilt, frazada, manta de polar), almohadas, cojines y maletas más chicas.

- **Inicio:** tres maletas grandes y tres chicas dibujadas, con la cantidad de cosas que tiene cada una. Abajo, la bandeja «Por guardar».
- **Diseñar:** elige tipo, tamaño (una plaza, una plaza y media, dos plazas), un color principal y, si quieres, otro color para el borde. La app dibuja la imagen y la deja en la bandeja.
- **Guardar:** arrastra un objeto de la bandeja a una maleta. Mantén presionada una maleta chica y arrástrala a una grande. Alternativa sin arrastrar: toca el objeto → «Mover a…», o abre una maleta y toca «Agregar».
- **Abrir:** toca una maleta; se abre con la tapa hacia arriba y muestra su interior visto desde arriba. Una maleta chica guardada se abre igual, tocándola. Para sacar algo, arrástralo a la barra inferior o tócalo → «Sacar a la bandeja».
- **Editar maletas:** lápiz dentro de una maleta (nombre, color, lunares, eliminar) y Ajustes → «Nueva maleta».
- **Datos:** solo en el iPhone (`localStorage`, clave `maletas.v1`). Ajustes → «Respaldo de datos» copia y restaura todo como texto.

## Publicación

GitHub Pages desde la rama `main`, carpeta raíz: Settings → Pages → Branch `main` / `(root)`. URL: https://pablocarvallo.github.io/maletas/

## Archivos

- `index.html`: toda la app (estilos, dibujos en SVG y código).
- `sw.js`: funciona sin conexión.
- `manifest.webmanifest` e `icons/`: instalación en la pantalla de inicio.
