# Práctica 1 - Sitio Web sobre Bob Dylan y Premios Nobel

## Descripción del Proyecto

Este proyecto es una página web sobre Bob Dylan y los Premios Nobel de Literatura. Está hecho con HTML, CSS y un poco de JavaScript para la navegación.

## Estructura del Proyecto

```
practica_1/
├── css/
│   └── estilos.css          # Archivo principal de estilos
├── img/
│   ├── Bob-Dylan-and-The-Band-1974.jpg
│   └── idioma.png
├── index.html               # Página principal sobre Bob Dylan
├── listado-nobel-literatura.html  # Lista de ganadores del Nobel
├── motivacion-premios.html  # Motivaciones de los premios
└── README.md               # Este archivo
```

## Páginas del Sitio

### 1. index.html - Página Principal
La página principal contiene un artículo sobre Bob Dylan y su Premio Nobel de Literatura. Incluye:
- Una imagen de Bob Dylan
- Un video de YouTube embebido
- Texto del artículo completo
- Enlaces a las otras páginas

### 2. listado-nobel-literatura.html - Lista de Premios
Esta página muestra una lista organizada de los ganadores del Premio Nobel de Literatura desde 2013 hasta 2022, agrupados por idioma de sus obras.

### 3. motivacion-premios.html - Motivaciones
Aquí se pueden ver las motivaciones oficiales de cada premio Nobel de Literatura.

## Entidades HTML Utilizadas

En este proyecto he usado varias entidades HTML importantes:

### Entidades de Caracteres Especiales
- `&aacute;` - á (a con acento agudo)
- `&eacute;` - é (e con acento agudo) 
- `&iacute;` - í (i con acento agudo)
- `&oacute;` - ó (o con acento agudo)
- `&uacute;` - ú (u con acento agudo)
- `&ntilde;` - ñ (eñe)
- `&uuml;` - ü (u con diéresis)
- `&quot;` - " (comillas dobles)
- `&amp;` - & (ampersand)

### Ejemplo de uso:
```html
<p>Bob Dylan recibi&oacute; el Premio Nobel de Literatura en 2016.</p>
```

## Estructura HTML Semántica

### Elementos Estructurales Principales

#### `<header>`
Contiene el encabezado de cada página con el título principal.

```html
<header>
    <h1>Bob Dylan y el Premio Nobel de Literatura</h1>
</header>
```

#### `<nav>`
Barra de navegación con enlaces a las diferentes páginas.

```html
<nav>
    <ul>
        <li><a href="index.html">Inicio</a></li>
        <li><a href="listado-nobel-literatura.html">Lista de Premios</a></li>
        <li><a href="motivacion-premios.html">Motivaciones</a></li>
    </ul>
</nav>
```

#### `<main>`
Contenido principal de cada página.

```html
<main>
    <article>
        <!-- Contenido del artículo -->
    </article>
</main>
```

#### `<footer>`
Pie de página con información del autor.

```html
<footer>
    <p>&copy; 2024 Jose Garcia. Todos los derechos reservados.</p>
</footer>
```

### Elementos de Contenido

#### Listas Anidadas
En la página de listado uso listas anidadas para organizar los premios por idioma:

```html
<ul>
    <li>Español
        <ul>
            <li><a href="motivacion-premios.html#mario-vargas-llosa">Mario Vargas Llosa (2010)</a></li>
        </ul>
    </li>
</ul>
```

#### Listas de Descripción
Para las motivaciones uso `<dl>`, `<dt>` y `<dd>`:

```html
<dl>
    <dt id="bob-dylan">Bob Dylan (2016)</dt>
    <dd>Por haber creado nuevas expresiones poéticas...</dd>
</dl>
```

#### Multimedia
- **Imágenes**: `<img>` con atributos alt para accesibilidad
- **Videos**: `<iframe>` para embeber videos de YouTube

```html
<img src="img/Bob-Dylan-and-The-Band-1974.jpg" alt="Bob Dylan en 1974">

<iframe src="https://www.youtube.com/embed/..." 
        title="Bob Dylan - Like a Rolling Stone">
</iframe>
```

## Características CSS

### Colores Utilizados
- Fondo: #ffffff (blanco)
- Texto principal: #333333 (gris oscuro)
- Enlaces: #0066cc (azul)
- Enlaces visitados: #800080 (morado)

### Tipografía
- Fuente principal: Arial, sans-serif
- Tamaños variables según la jerarquía (h1, h2, p, etc.)

### Responsive Design
El sitio se adapta a pantallas pequeñas con media queries:

```css
@media (max-width: 768px) {
    .container {
        padding: 10px;
    }
}
```

## Navegación

Todas las páginas están conectadas mediante:
- Menú de navegación principal
- Enlaces internos con anclas (#)
- Enlaces externos a sitios oficiales

## Cómo Ver el Proyecto

1. Abrir una terminal en la carpeta del proyecto
2. Ejecutar: `python -m http.server 8000`
3. Ir a: http://localhost:8000

## Notas del Desarrollador

Este proyecto fue creado como práctica de HTML y CSS básico. Incluye todas las funcionalidades requeridas y está optimizado para ser funcional y visualmente atractivo.

---

**Autor**: Joseph Z. Gaitán Mosquera  
**Fecha**: 2025  
**Asignatura**: Interfaces Gráficas