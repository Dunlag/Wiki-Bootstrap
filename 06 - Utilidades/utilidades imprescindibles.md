# Guía de Utilidades en Bootstrap

Bootstrap proporciona una serie de clases de utilidad para aplicar estilos rápidamente sin necesidad de CSS adicional. A continuación, se explican las más utilizadas con ejemplos.

---

## Opacidad

La clase `opacity-{valor}` permite ajustar la opacidad de un elemento. Los valores disponibles son `100`, `75`, `50`, y `25`.

```html
<div class="opacity-100 bg-success">100%</div>
<div class="opacity-75 bg-success">75%</div>
<div class="opacity-50 bg-success">50%</div>
<div class="opacity-25 bg-success">25%</div>
```

**💡 Consejo:** Útil para crear efectos de transparencia en fondos o imágenes superpuestas.

---

## Posicionamiento

Define la posición de un elemento:

- `position-static` (Posición por defecto)
- `position-relative` (Posición relativa a su posición original)
- `position-absolute` (Posición absoluta respecto al contenedor más cercano con `position: relative`)
- `position-fixed` (Fijo en la pantalla)
- `position-sticky` (Pegajoso hasta alcanzar un límite)

```html
<div class="position-relative bg-warning p-3">Elemento Relativo</div>
<div class="position-absolute bg-danger p-3">Elemento Absoluto</div>
```

**💡 Consejo:** Usa `position-sticky` para mantener elementos visibles al hacer scroll, como una barra de navegación.

---

## Visibilidad

Para controlar la visibilidad de un elemento:

- `visible`: Hace visible un elemento.
- `invisible`: Oculta el elemento pero mantiene su espacio.

```html
<div class="visible bg-primary">Visible</div>
<div class="invisible bg-secondary">Invisible</div>
```

**💡 Consejo:** `invisible` es útil para ocultar elementos sin afectar el diseño.

---

## Margen y Relleno (Margin & Padding)

Se pueden aplicar márgenes (`m-{valor}`) y rellenos (`p-{valor}`):

```html
<div class="m-3 p-3 bg-info">Margen y Padding</div>
```

Valores comunes:

- `0` (Sin espacio)
- `1` (0.25rem)
- `2` (0.5rem)
- `3` (1rem)
- `4` (1.5rem)
- `5` (3rem)

**💡 Consejo:** Usa `mx-auto` para centrar horizontalmente elementos con `display: block`.

---

## Flotantes (Float)

Las clases `float-{start|end|none}` permiten flotar elementos.

```html
<img src="img.jpg" class="float-end" alt="Imagen flotante">
```

**💡 Consejo:** Usa `clearfix` en el contenedor padre para evitar problemas con elementos flotantes.

---

## Colores de Texto

Aplica colores con `text-{color}`:

```html
<p class="text-primary">Texto Azul</p>
<p class="text-danger">Texto Rojo</p>
```

---

## Fondos

Aplica colores de fondo con `bg-{color}`:

```html
<div class="bg-success p-3">Fondo Verde</div>
```

**💡 Consejo:** Puedes combinarlo con `text-white` para mejorar la legibilidad.

---

## Bordes

Para agregar bordes:

```html
<div class="border border-primary p-3">Borde Azul</div>
```

**💡 Consejo:** Usa `rounded` para bordes redondeados.

---

## Textos

Alinear, modificar tamaño y peso del texto:

```html
<p class="text-center">Texto centrado</p>
<p class="fs-1">Texto grande</p>
<p class="fw-bold">Texto en negrita</p>
```

---

## Anchos y Altos

Definir tamaño de elementos:

```html
<div class="w-50 bg-secondary">50% de ancho</div>
<div class="h-25 bg-dark">25% de altura</div>
```

**💡 Consejo:** Usa `vh-100` para establecer altura completa de la pantalla.

---

Esta guía cubre las utilidades más usadas en Bootstrap. ¡Experimenta combinándolas para mejorar tus diseños! 🚀

