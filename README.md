# Maletas

App web para iPhone que organiza lo que guardas en tus maletas: mantas (quilt, frazada, manta de polar), almohadas, cojines y maletas más chicas.

- **Inicio:** tres maletas grandes y tres chicas dibujadas, con la cantidad de cosas que tiene cada una. Abajo, la bandeja «Por guardar».
- **Diseñar:** elige qué es (manta, almohada, cojín, cuello o mochila), el tipo, el tamaño, un color principal y, si quieres, otro color para el borde, el broche o los bolsillos. La app dibuja la imagen y la deja en la bandeja.
- **Guardar:** arrastra un objeto de la bandeja a una maleta. Mantén presionada una maleta chica y arrástrala a una grande. Alternativa sin arrastrar: toca el objeto → «Mover a…», o abre una maleta y toca «Agregar».
- **Abrir:** toca una maleta; se abre con la tapa hacia arriba y muestra su interior visto desde arriba. Una maleta chica guardada se abre igual, tocándola. Para sacar algo, arrástralo a la barra inferior o tócalo → «Sacar a la bandeja».
- **Editar maletas:** lápiz dentro de una maleta (nombre, color, lunares, estampado desde foto, eliminar).
- **Datos:** solo en el iPhone (`localStorage`, clave `maletas.v1`). Ajustes → «Respaldo de datos» copia y restaura todo como texto.

## Publicación

GitHub Pages desde la rama `main`, carpeta raíz: Settings → Pages → Branch `main` / `(root)`. URL: https://pablocarvallo.github.io/maletas/

## Archivos

- `index.html`: toda la app (estilos, dibujos en SVG y código).
- `sw.js`: funciona sin conexión.
- `manifest.webmanifest` e `icons/`: instalación en la pantalla de inicio.
- **Estampado desde una foto:** en el editor de una maleta, «Usar una foto como estampado»: se elige un recorte de la foto (posición y tamaño) y se aplica cubriendo la maleta o repetido en mosaico. Se guarda solo el recorte, reducido, dentro de los datos de la app (y del respaldo).
- **Diseño de objetos desde una foto:** en el diseñador, «Tomar el diseño de una foto» aplica un recorte de la foto como tela del objeto (manta, almohada, cojín, cuello o mochila), cubriendo o en mosaico. Se guarda solo el recorte reducido.
- **Proporciones y llenado visual:** la maleta grande (bodega, 23 kg) se dibuja con proporciones de 75×50×30 cm y la chica (cabina) de 55×40×20 cm, a la misma escala. El interior se ve desde arriba y los objetos se acomodan por capas según su tamaño, así que la maleta se ve más llena a medida que se guarda más. La lista «Contenido» permite tocar o arrastrar objetos que quedan tapados. Los tamaños de los objetos son aproximaciones típicas.
