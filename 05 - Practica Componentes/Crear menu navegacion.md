# Guía de Menús de Navegación en Bootstrap

Bootstrap proporciona una forma sencilla de crear barras de navegación (navbars) responsivas y estilizadas. En esta guía aprenderás a construir un menú de navegación funcional y personalizable.

## 1. Estructura Básica de un Navbar

Un `navbar` en Bootstrap utiliza la clase `navbar` junto con `navbar-expand-lg` para definir su comportamiento responsivo. Aquí tienes un ejemplo básico:

```html
<nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
        <a class="navbar-brand" href="#">Mi sitio web</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a href="#" class="nav-link active">Home</a>
                </li>
                <li class="nav-item">
                    <a href="#" class="nav-link">Link</a>
                </li>
                <li class="nav-item">
                    <a href="#" class="nav-link disabled">Contacto</a>
                </li>
            </ul>
        </div>
    </div>
</nav>
```

### Explicación:
- `navbar`: Define la barra de navegación.
- `navbar-expand-lg`: Indica que el menú se expandirá en dispositivos grandes.
- `bg-body-tertiary`: Define un color de fondo.
- `container-fluid`: Permite que el contenido se expanda por toda la pantalla.
- `navbar-toggler`: Botón para mostrar u ocultar el menú en dispositivos pequeños.

## 2. Agregar Elementos al Menú

Puedes añadir elementos como botones, formularios y desplegables dentro del `navbar`.

### Agregar un Menú Desplegable

```html
<li class="nav-item dropdown">
    <a href="#" class="nav-link dropdown-toggle" data-bs-toggle="dropdown">Desplegable</a>
    <ul class="dropdown-menu">
        <li><a href="#" class="dropdown-item">Link1</a></li>
        <li><a href="#" class="dropdown-item">Link2</a></li>
    </ul>
</li>
```

### Agregar un Formulario de Búsqueda

```html
<form class="d-flex">
    <input type="text" class="form-control" placeholder="Buscar">
    <button class="btn btn-outline-success">Buscar</button>
</form>
```

## 3. Personalización con Clases de Bootstrap

Puedes modificar la apariencia del `navbar` usando clases adicionales:
- `bg-light`, `bg-dark`: Cambian el color de fondo.
- `navbar-light`, `navbar-dark`: Ajustan el color del texto según el fondo.
- `fixed-top`, `fixed-bottom`: Fijan el menú en la parte superior o inferior.

Ejemplo con fondo oscuro:

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
```

## 4. Consejos y Buenas Prácticas

- **Usar `container` o `container-fluid`**: Ayuda a mantener el diseño responsivo.
- **Colocar `navbar-toggler` correctamente**: Asegura que el menú sea accesible en dispositivos móviles.
- **Cargar Bootstrap antes de tu JavaScript personalizado**: Evita errores al manipular componentes como `dropdown` o `modal`.
- **Agregar clases de alineación como `me-auto`**: Controla la distribución de elementos en el navbar.

## 5. Carga de Bootstrap y JavaScript

Para que los componentes interactivos funcionen correctamente, recuerda incluir los scripts de Bootstrap:

```html
<script src="./node_modules/@popperjs/core/dist/umd/popper.min.js"></script>
<script src="./node_modules/bootstrap/dist/js/bootstrap.js"></script>
```

---


