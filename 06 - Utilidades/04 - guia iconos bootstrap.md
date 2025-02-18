# Guía de Iconos en Bootstrap

Bootstrap ofrece una gran cantidad de iconos que pueden utilizarse fácilmente en proyectos web. En esta guía, aprenderás cómo instalar, usar y personalizar los iconos de Bootstrap.

## Instalación de Bootstrap Icons

Para instalar los iconos de Bootstrap con npm, ejecuta el siguiente comando:

```sh
npm i bootstrap-icons
```

Luego, importa el archivo CSS en tu proyecto:

```html
<link rel="stylesheet" href="./node_modules/bootstrap-icons/font/bootstrap-icons.css">
```

---

## Uso Básico de Iconos

Para añadir un icono, simplemente usa la clase correspondiente de Bootstrap dentro de un elemento `<i>`:

```html
<i class="bi bi-airplane-engines"></i>
<i class="bi bi-ubuntu"></i>
<i class="bi bi-windows"></i>
<i class="bi bi-twitch"></i>
<i class="bi bi-xbox"></i>
```

✅ **Consejo:** Puedes modificar el tamaño de los iconos usando clases como `fs-1`, `fs-2`, etc.

```html
<i class="bi bi-star-fill fs-1"></i>
<i class="bi bi-star-fill fs-3"></i>
```

---

## Iconos en Botones

Los iconos pueden mejorar la accesibilidad visual de los botones:

```html
<button class="btn btn-primary">
    <i class="bi bi-check-circle"></i> Confirmar
</button>

<button class="btn btn-danger">
    <i class="bi bi-trash"></i> Eliminar
</button>
```

✅ **Consejo:** Usa `me-2` o `ms-2` para espaciar el icono del texto:

```html
<button class="btn btn-success">
    <i class="bi bi-download me-2"></i> Descargar
</button>
```

---

## Iconos en Formularios y Barras de Búsqueda

Puedes añadir iconos dentro de los `input-group` para mejorar la experiencia de usuario:

```html
<div class="input-group mb-3">
    <span class="input-group-text"><i class="bi bi-search"></i></span>
    <input type="text" class="form-control" placeholder="Buscar...">
</div>
```

✅ **Consejo:** Usa iconos relevantes para mejorar la usabilidad en formularios.

```html
<div class="input-group mb-3">
    <input type="text" class="form-control" placeholder="Correo electrónico">
    <span class="input-group-text"><i class="bi bi-envelope"></i></span>
</div>
```

---

## Listas con Iconos

Los iconos pueden utilizarse en listas para hacerlas más intuitivas:

```html
<ul class="list-group">
    <li class="list-group-item"><i class="bi bi-star-fill text-warning"></i> Favoritos</li>
    <li class="list-group-item"><i class="bi bi-person-fill text-primary"></i> Perfil</li>
    <li class="list-group-item"><i class="bi bi-gear-fill text-secondary"></i> Configuración</li>
</ul>
```

---

## Enlaces con Iconos

Puedes añadir iconos a enlaces para mejorar la navegación:

```html
<a href="#" class="text-decoration-none">
    <i class="bi bi-arrow-right"></i> Más información
</a>
```

✅ **Consejo:** Usa `text-decoration-none` para evitar el subrayado en los enlaces.

---


Para explorar más iconos, visita la [documentación oficial de Bootstrap Icons](https://icons.getbootstrap.com/).

