# SistemasCorrelativas

Correlativas de Ingeniería en Sistemas de Información (Plan 2023) de la UTN FRC.

App web para seguir el avance de la carrera: marcás cada materia como **Regular** o **Aprobada** y se calcula solo qué materias podés cursar según la tabla de correlativas.

## Qué hace

- Muestra el plan por niveles (1 a 5), las electivas y el Seminario Integrador. El Seminario está en una sección aparte porque solo se necesita para el título intermedio de Analista.
- Calcula el estado de cada materia: aprobada, regular, cursable o no cursable.
- Al tocar una materia muestra qué correlativas pide, cuáles te faltan para rendir el final y qué materias habilita.
- Guarda las notas finales y los aplazos, y calcula el promedio con y sin aplazos.
- Lleva la cuenta de los créditos electivos (Ingeniería pide 20).
- Tiene filtros y buscador.

## Uso

Abrí `index.html` en el navegador o publicá la carpeta en cualquier hosting estático (por ejemplo GitHub Pages). Es una PWA: se puede instalar en el celular y funciona sin internet.

Los datos se guardan solo en el navegador (`localStorage`). Para pasarlos a otro dispositivo, usá **Copiar respaldo** y después **Restaurar desde el código**.

## Archivos

- `index.html`: la app completa (HTML, CSS y JS en un solo archivo).
- `sw.js`: service worker para que funcione sin conexión. Si cambiás `index.html`, subí la versión del caché (`correlativas-vN`) para que los celulares descarguen la versión nueva.
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`: datos para instalar la app.
