# Componentes Complejos en Bootstrap

Bootstrap ofrece una serie de componentes que combinan varios elementos HTML y requieren scripts adicionales para su funcionalidad. En esta sección exploraremos algunos de ellos, cómo funcionan y cómo pueden ser modificados.

## Uso de Popper.js

Algunos de los componentes de Bootstrap, como los dropdowns y tooltips, dependen de [Popper.js](https://popper.js.org/) para gestionar el posicionamiento de los elementos emergentes. Para que estos funcionen correctamente en un entorno de desarrollo local con Node.js, es necesario incluir Popper.js manualmente con:

```html
<script src="./node_modules/@popperjs/core/dist/umd/popper-base.js"></script>
```

Popper.js permite:
- Posicionar elementos emergentes de manera automática y precisa.
- Gestionar colisiones con otros elementos en pantalla.
- Ofrecer opciones avanzadas de alineación y animación.

---

## Dropdowns en Bootstrap

Un **dropdown** es un menú desplegable que se activa al hacer clic en un botón. Para usarlo correctamente:

```html
<div class="dropdown">
    <button class="btn btn-danger dropdown-toggle" data-bs-toggle="dropdown">
        Mi listado
    </button>
    <ul class="dropdown-menu">
        <li><a href="#" class="dropdown-item">Item 1</a></li>
        <li><hr class="dropdown-divider"></li>
        <li><a href="#" class="dropdown-item">Item 2</a></li>
    </ul>
</div>
```

### Personalización
Puedes cambiar el color del botón usando las clases `btn-primary`, `btn-warning`, etc., y modificar la dirección del desplegable con `dropend`, `dropstart`, o `dropup`.

---

## Navegación (Navs)

Los elementos de navegación pueden presentarse de diferentes formas:

```html
<ul class="nav justify-content-center">
    <li class="nav-item"><a href="#" class="nav-link">Opcion 1</a></li>
    <li class="nav-item"><a href="#" class="nav-link">Opcion 2</a></li>
    <li class="nav-item"><a href="#" class="nav-link disabled">Opcion 3</a></li>
</ul>
```

Para resaltar la opción activa, usa `active`:
```html
<a href="#" class="nav-link active">Activa</a>
```

Y para transformar la navegación en pestañas o píldoras:
```html
<ul class="nav nav-pills">
    <li class="nav-item"><a href="#" class="nav-link">Pestaña 1</a></li>
</ul>
```

---

## Tarjetas (Cards)

Las **cards** en Bootstrap son contenedores flexibles con estructura definida:

```html
<div class="card">
    <div class="card-header">Cabecera</div>
    <div class="card-body text-bg-danger">
        Contenido principal de la tarjeta.
    </div>
    <div class="card-footer">Pie de tarjeta</div>
</div>
```

Puedes agregar **imágenes**, **botones** y otros elementos dentro de la tarjeta.

---

## Modales (Modal)

Los modales permiten mostrar ventanas emergentes en pantalla:

```html
<div class="modal fade" id="exampleModal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <h1 class="modal-title">Título Modal</h1>
                <button class="btn-close" data-bs-dismiss="modal"></button>
            </div>
            <div class="modal-body">Contenido del modal</div>
            <div class="modal-footer">
                <button class="btn btn-secondary" data-bs-dismiss="modal">Cerrar</button>
            </div>
        </div>
    </div>
</div>
<button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">Abrir</button>
```

Puedes modificar su tamaño con clases como `modal-lg` o `modal-sm` en `modal-dialog`.

---

## Conclusión

Estos son algunos de los componentes complejos de Bootstrap. Puedes personalizarlos con CSS, clases adicionales o combinarlos para crear diseños interactivos. Explora la [documentación oficial](https://getbootstrap.com/) para descubrir más opciones y ejemplos.

