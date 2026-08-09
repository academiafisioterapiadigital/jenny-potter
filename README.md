# Jenny Potter y el Colocón Filosofal

Grimorio interactivo para la despedida de soltera de Jenny.
Web estática: HTML, CSS y JavaScript en un solo archivo, sin dependencias ni build.

## Estructura

```
index.html        toda la experiencia (estilos y lógica incluidos)
media/            imágenes y vídeo
```

## Publicarlo en GitHub Pages

1. Crea un repositorio nuevo en GitHub y sube estos archivos a la raíz.
2. En el repo: **Settings → Pages**.
3. En *Source* elige **Deploy from a branch**, rama `main`, carpeta `/root`. Guarda.
4. En dos o tres minutos estará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

Alternativas sin GitHub: arrastrar la carpeta a [netlify.com/drop](https://app.netlify.com/drop)
o a Vercel. Publican en segundos y dan una URL igual de válida.

## Cambiar la foto de Jenny por un vídeo

El veredicto del Sombrero acepta vídeo en bucle. Guarda tu archivo como:

- `media/jenny.mp4` — H.264, imprescindible para iPhone
- `media/jenny.webm` — opcional, pesa menos en Android y escritorio

Se reproduce solo, en bucle y sin sonido. Si no existe ninguno de los dos,
la página muestra automáticamente `media/jenny.jpg` y no se rompe nada.

Recomendaciones: vertical (relación 2:3), entre 3 y 8 segundos, menos de 5 MB.
Mantén `media/jenny.jpg` como primer fotograma: es lo que se ve mientras carga.

## Editar el contenido

Todo el texto está al final de `index.html`, dentro del `<script>`:

- `PREGUNTAS` — las cuatro preguntas del Sombrero y sus opciones
- `MURMULLOS` — lo que dice mientras delibera
- `CAPS` — los cuatro capítulos: horarios, notas, retos y citas

El veredicto siempre es Gryffindor, decida ella lo que decida.
