### Guía en Markdown sobre los componentes básicos


# Guía de Componentes Básicos de Bootstrap

Esta guía cubre algunos de los componentes básicos más utilizados de **Bootstrap**, como botones, alertas, badges, y listas, basándonos en un ejemplo práctico.

## 1. Botones

Bootstrap proporciona una gran cantidad de botones estilizados con clases predefinidas. Aquí mostramos ejemplos de varios tipos de botones.

### Botones con colores predefinidos

Bootstrap viene con varias clases de color que se pueden aplicar fácilmente a los botones. Aquí hay algunos ejemplos:

```html
<button type="button" class="btn btn-primary">Botón Primary</button>
<button type="button" class="btn btn-secondary">Botón Secondary</button>
<button type="button" class="btn btn-success">Botón Success</button>
<button type="button" class="btn btn-danger">Botón Danger</button>
<button type="button" class="btn btn-warning">Botón Warning</button>
<button type="button" class="btn btn-info">Botón Info</button>
<button type="button" class="btn btn-light">Botón Light</button>
<button type="button" class="btn btn-dark">Botón Dark</button>
```

### Botón de enlace

Se puede usar el estilo de botón para crear enlaces estilizados como botones:

```html
<button type="button" class="btn btn-link">Botón Link</button>
```

### Botones Outline

Bootstrap permite crear botones con borde (outline), que pueden ser útiles para diseñar interfaces más ligeras.

```html
<button type="button" class="btn btn-dark btn-outline-danger">Botón Dark</button>
<button type="button" class="btn btn-warning btn-outline-secondary">Botón warning</button>
```

### Tamaños de Botones

Puedes ajustar el tamaño de los botones usando las clases `btn-sm` y `btn-lg`:

```html
<button type="button" class="btn btn-dark btn-sm">Botón pequeño</button>
<button type="button" class="btn btn-dark btn">Botón mediano</button>
<button type="button" class="btn btn-dark btn-lg">Botón grande</button>
```

### Botones agrupados

Bootstrap ofrece la opción de agrupar botones, lo que es útil para crear un conjunto de botones relacionados, como botones de acción o opciones.

```html
<div class="btn-group">
    <button type="button" class="btn btn-primary">Botón Primary</button>
    <button type="button" class="btn btn-secondary">Botón Secondary</button>
    <button type="button" class="btn btn-success">Botón Success</button>
    <button type="button" class="btn btn-danger">Botón Danger</button>
</div>
```

## 2. Alertas

Las alertas se utilizan para mostrar mensajes importantes al usuario. Bootstrap ofrece varios tipos de alertas con diferentes niveles de gravedad.

### Tipos de Alertas

```html
<div class="alert alert-success">Alerta</div>
<div class="alert alert-primary">Alerta</div>
<div class="alert alert-danger">Alerta</div>
```

### Alerta con encabezado y botón de cierre

Puedes personalizar las alertas con un encabezado y un botón para cerrarlas.

```html
<div class="alert alert-danger">
    <h4 class="alert-heading">tituloAlerta heading</h4>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
    <button type="button" class="btn-close" data-bs-dismiss='alert'></button>
</div>
```

## 3. Badge

Los "badges" o insignias se usan para mostrar pequeñas cantidades de información adicional, como contadores.

```html
<button class="btn btn-primary">
    Mensaje <span class="badge text-bg-secondary rounded-pill">3</span>
</button>
```

## 4. Listas de grupo

Las listas de grupo son útiles para mostrar elementos listados con opciones de estilo, como elementos activos, deshabilitados, etc.

```html
<ul class="list-group">
    <li class="list-group-item active">Primero</li>
    <li class="list-group-item">segundo</li>
    <li class="list-group-item disabled">tercero</li>
</ul>
```

---

### Consejos adicionales

1. **Consistencia en los estilos**: Asegúrate de usar los mismos estilos y clases en todos los componentes relacionados para mantener una interfaz consistente.

2. **Comodidad en el diseño**: Si usas muchos botones, considera utilizar `btn-group` para agruparlos y evitar que se vean desordenados.

3. **Alertas con interacción**: Puedes agregar un botón de cierre a las alertas con la clase `btn-close` para mejorar la interacción del usuario.

4. **Responsive**: Los componentes de Bootstrap son completamente **responsivos**, lo que significa que se ajustan automáticamente en pantallas de diferentes tamaños.

