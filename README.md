# Título del proyecto
Breve descripción del sitio web y de su temática.
## Autoría
- Nombre y apellidos: Anthony Cristian Morar
- Curso: 1º
- Módulo: DAMA
- Fecha:15/11/2026
## Sitio publicado
- Web en GitHub Pages: [Abrir sitio](https://anthmor.github.io/CotilleosCiencia/)
- Repositorio: [Abrir repositorio](https://github.com/Anthmor/CotilleosCiencia)
## Estructura del proyecto
- `index.html`: página principal con la presentación del proyecto, resúmenes de contenidos y enlaces externos.
- `blog.html`: artículo extenso sobre la disputa entre Isaac Newton y Robert Hooke utilizando etiquetas semánticas de bloque y de texto.
- `tabla.html`: tabla accesible con `caption`, `thead`, `tbody`, `tfoot`, `scope`, `colspan` y `rowspan` sobre controversias científicas.
- `galeria.html`: galería de nueve piezas gráficas en distintos formatos, mapa de imagen interactivo, vídeo local con subtítulos, audios locales y contenido externo incrustado.
- `formulario.html`: formulario de colaboración con tres grupos `fieldset`, controles etiquetados y validación nativa HTML5.
- `rss.xml`: canal de sindicación RSS 2.0 con los contenidos principales del sitio.
- `css/estilos.css`: hoja de estilos externa compartida por las cinco páginas.
- `img/`, `audio/`, `video/`: carpetas organizadas para recursos multimedia y pistas WebVTT.
## Tecnologías utilizadas
- HTML5
- CSS
- XML y RSS
- Git
LMSGI UD 2. HTML 5
- GitHub
- GitHub Pages
## Características principales
- Navegación entre cinco páginas.
- Uso de HTML semántico.
- Tabla accesible.
- Galería con varios formatos.
- Contenido multimedia.
- Formulario con validación HTML.
- Canal RSS.
## Validación
### HTML
![Resultado de validación HTML](img/validacion-html.png)
### CSS
![Resultado de validación CSS](img/validacion-css.png)
### RSS
![Resultado de validación RSS](img/validacion-rss.png)

## Dificultades encontradas
Describe al menos tres dificultades reales:
1. Coordenadas exactas en el mapa de imagen: Al definir las zonas clicables (`rect`, `circle` y `poly`) en `galeria.html`, las coordenadas iniciales no coincidían con las figuras visuales. Se resolvió diseñando primero el gráfico SVG con dimensiones fijas (`600x300`) y trasladando exactamente los vértices y radios de cada figura al atributo `coords`.
2. Sensibilidad a mayúsculas y minúsculas en rutas: En local algunas rutas funcionaban aunque no coincidieran exactamente las letras, pero en servidores Linux como GitHub Pages pueden fallar. Se revisaron todos los archivos y carpetas para mantenerlos estrictamente en minúsculas y con rutas relativas.
3. Validación de tablas complejas y fechas RSS: Durante la validación se ajustaron los atributos `scope="colgroup"` en encabezados combinados y el formato estándar RFC-822 en las etiquetas `<pubDate>` del canal `rss.xml` hasta lograr cero errores.

## Decisiones técnicas
Explica brevemente:
Organización de archivos: Separación clara por tipo de recurso (`css/`, `img/`, `audio/`, `video/`, `subtitulos/`) y nombres descriptivos sin espacios ni caracteres especiales.
- Plantilla común frente a contenido variable: Se mantienen idénticos el `header`, el menú de navegación (`nav`) y el `footer` en las cinco páginas, cambiando únicamente el `<title>`, la marca de página activa, el `<h1>` y el contenido de `<main>`.
- Elección de formatos de imagen: Se empleó JPG para fotografías con gran riqueza cromática, WebP para mejorar la compresión web, PNG para elementos que requieren transparencia sobre cualquier fondo, y SVG tanto para el logotipo e iconos vectoriales escalables como para una animación ligera sin JavaScript.
- Preparación para la práctica de CSS: Todas las páginas enlazan una única hoja `css/estilos.css` y evitan atributos obsoletos o estilos en línea, separando completamente la estructura del diseño visual.

## Fuentes y licencias
- Textos históricos: Redacción propia basada en documentación divulgativa pública (Archivos de The Royal Society y CSIC).
- Gráficos vectoriales (`logo.svg`, `favicon.svg`, `balanza-vectorial.svg`, `atomo-animado.svg`, `mapa-laboratorio.svg`, `separador-decorativo.svg`) y subtítulos (`.vtt`): Creación propia para esta práctica educativa.
- Fotografías, audios y vídeo local: Recursos obtenidos de bancos con licencia libre / Dominio Público (Wikimedia Commons / Pixabay) Excepto videos recogidos de [https://www.youtube.com/watch?v=QqsLTNkzvaY]; [https://www.youtube.com/watch?v=3L40vUClfjU] *Sin licencia libre*.
