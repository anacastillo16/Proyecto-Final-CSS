# Proyecto Final CSS

## Resumen del proyecto
Este proyecto consta de 4 páginas html, las 3 primeras realizadas con HTML y CSS y la última con HTML y Bootstrap. Es el proyecto final de la asignatura "Diseño de Interfaces WEB" de 2º de DAW, donde hemos usado todas las herramientas aprendidas durante todo el curso. 

## Estructura del proyecto
### Cabecera

- El logotipo tiene un enlace a `index.html`.
- El menú de navegación está compuesto por tres ítems:
  - "Películas" (enlace a `pelis.html`).
  - "Series" (enlace a `series.html`).
  - "Trailers" (enlace a `trailers.html`).
- Al pasar el cursor sobre los enlaces (estado hover), aparece una línea debajo de ellos y el cursor se convierte en forma de mano.
- El diseño está realizado con Flexbox (HTML y CSS).

### Footer

- El pie de página tiene dos bloques:
  1. En el primer bloque (izquierda), se encuentran el logotipo y mi nombre completo.
  2. En el segundo bloque (derecha), hay dos filas:
     - Fila superior: una lista con iconos de tres redes sociales (con enlaces vacíos).
     - Fila inferior: un menú con tres ítems (con enlaces vacíos): "Política de privacidad", "Política de cookies", "Aviso legal".
- Al pasar el cursor sobre los enlaces (estado hover), aparece una línea debajo de ellos y el cursor se convierte en forma de mano.
- El diseño está hecho con Flexbox (HTML y CSS).

### Página `index.html`

- La página contiene la cabecera y el footer previamente descritos.
- El contenido principal tiene:
  - Un `<div>` con una imagen de banner y un formulario de suscripción.
  - Una `<section>` con dos `<article>`, uno para una película y otro para una serie, cada uno con un botón "Ver más". Los botones enlazan con `pelis.html` y `series.html` respectivamente.

### Página `pelis.html`

- La página contiene la cabecera y el footer previamente descritos.
- El contenido principal tiene:
  - Un `<div>` con un buscador (que no tiene funcionalidad ya que no se ha implementado JavaScript).
  - Una `<section>` con varios `<article>`, cada uno mostrando una película con una imagen, año de estreno y una breve descripción. Además, cada artículo tiene un botón (sin funcionalidad).
  - El diseño del `<section>` está realizado con Grid (HTML y CSS).

### Página `series.html`

- La página contiene la cabecera y el footer previamente descritos.
- El contenido principal tiene:
  - Un `<div>` con un buscador (sin funcionalidad).
  - Una `<section>` con varios `<article>`, cada uno mostrando una serie con una imagen, año de estreno, número de temporadas y una breve descripción. También contiene un botón (sin funcionalidad).
  - El diseño del `<section>` está realizado con Grid (HTML y CSS).

### Página `trailers.html`

- La página contiene la cabecera y el footer previamente descritos, pero en este caso utilizando Bootstrap 5.
- El contenido principal tiene:
  - Un `<main>` con varios `<div>` que muestran tráileres de películas y series. Los `<div>` son tarjetas de Bootstrap.

## Selectores escogidos y su justificación
1. **Selectores de ID (`#`)**:
   - Se utilizan para elementos únicos en la página que requieren estilos específicos.
   - Ejemplos: `#logo`, `#banner`, `#sectionINDEX`, `#articulo1`, `#articulo2`, `#h1Pelis`, `#buscador`, `#peliculas`.

2. **Selectores de clase (`.`)**:
   - Se usan para aplicar estilos a grupos de elementos que comparten características comunes.
   - Ejemplos: `.articuloINDEX`, `.contenido`, `.boton`, `.footer-left`, `.footer-right`, `.footer-socials`, `.footer-links`, `.pelicula`, `.texto`, `.year`.

3. **Selectores de elemento**:
   - Permiten aplicar estilos generales a todos los elementos de un tipo específico.
   - Ejemplos: `header`, `nav`, `ul`, `li`, `a`, `main`, `section`, `article`, `h1`, `h3`, `h4`, `p`, `img`, `form`, `input`, `button`, `footer`.

4. **Pseudo-clases**:
   - Se utilizan para aplicar estilos en estados específicos de los elementos, mejorando la interactividad.
   - Ejemplos: `:hover` (para enlaces y botones), `:focus` (para inputs de formularios).

## Colores utilizados en la confección del sitio
| Elemento                   | RGB                |
|-----------------------------|--------------------|
| Fondo header                | rgb(187, 225, 247) |
| Texto general y enlaces     | rgb(0, 0, 0)       |
| Fondo de artículos          | #f4f4f4            |
| Borde de artículos          | rgb(187, 225, 247) |
| Título de películas/series, Hover de botones, Botón del buscador | rgb(167, 167, 255) |
| Fondo de botones            | rgb(187, 225, 247) |
| Fondo del buscador          | #ffffff            |
| Hover botón buscador        | rgb(145, 145, 230) |
| Texto de párrafos           | #333               |
| Fondo del footer            | rgb(187, 225, 247) |

## Aspecto de los enlaces
1. **Menú de navegación principal**:
   - Color normal: Negro (`#000`).
   - Estado `:hover`: Negro con subrayado.

2. **Botones**:
   - Color normal: Negro sobre fondo rgb(187, 225, 247).
   - Estado `:hover`: Negro sobre fondo rgb(167, 167, 255).

3. **Enlaces del pie de página**:
   - Color normal: Negro (`#000`).
   - Estado `:hover`: Negro con subrayado.

## Medias Querys
1. **Pequeño (SM)** - Móviles:
   ```css
   @media (min-width: 400px) and (max-width: 768px) {}
2. **Mediano (MD)** - Tablets:
   ```css
   @media (min-width: 769px) and (max-width: 992px) {}
3. **Grande (LG)** - Laptops, monitores, pantallas grandes:
   ```css
   @media (min-width: 993px) and (max-width: 1200px) {}
