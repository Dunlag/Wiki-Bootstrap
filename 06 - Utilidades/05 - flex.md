# 📌 Guía de Flexbox en Bootstrap

Bootstrap proporciona una serie de clases para trabajar con Flexbox y hacer que el diseño sea más adaptable y dinámico. En esta guía, exploraremos las clases más importantes y cómo usarlas con ejemplos.

---

## 🎯 1. Clases Básicas de Flexbox

Para habilitar flexbox en un contenedor, usa la clase `d-flex`.

```html
<div class="d-flex bg-light p-3">
    <div class="bg-primary text-white p-3">Item 1</div>
    <div class="bg-secondary text-white p-3">Item 2</div>
    <div class="bg-success text-white p-3">Item 3</div>
</div>
```

🔹 **Consejo:** La clase `d-flex` aplica `display: flex;` al contenedor.

---

## 📌 2. Dirección del Contenido

### ▶️ `flex-row` y `flex-row-reverse`

```html
<div class="d-flex flex-row">
    <div class="p-3 bg-info">1</div>
    <div class="p-3 bg-warning">2</div>
    <div class="p-3 bg-danger">3</div>
</div>
```

🔄 Usa `flex-row-reverse` para invertir el orden.

### 🔽 `flex-column` y `flex-column-reverse`

```html
<div class="d-flex flex-column">
    <div class="p-3 bg-info">1</div>
    <div class="p-3 bg-warning">2</div>
    <div class="p-3 bg-danger">3</div>
</div>
```

🔄 `flex-column-reverse` invierte el orden de los elementos en columna.

---

## 🔄 3. Flex-Wrap: Controlando el ajuste

### ✅ `flex-wrap`

```html
<div class="d-flex flex-wrap">
    <div class="p-3 bg-success w-25">1</div>
    <div class="p-3 bg-danger w-25">2</div>
    <div class="p-3 bg-warning w-25">3</div>
    <div class="p-3 bg-info w-25">4</div>
</div>
```

📢 **TIP:** Usa `flex-nowrap` para evitar que los elementos se desborden a la siguiente línea.

---

## ⚖️ 4. Crecimiento y reducción de elementos

### 📈 `flex-grow`

```html
<div class="d-flex">
    <div class="p-3 bg-success flex-grow-1">A</div>
    <div class="p-3 bg-danger">B</div>
    <div class="p-3 bg-warning flex-grow-1">C</div>
</div>
```

### 📉 `flex-shrink`

```html
<div class="d-flex">
    <div class="p-3 bg-success flex-shrink-1">X</div>
    <div class="p-3 bg-danger">Y</div>
    <div class="p-3 bg-warning">Z</div>
</div>
```

📢 **Consejo:** `flex-grow-0` evita que un elemento crezca.

---

## 🔀 5. Alineación de elementos

### 🏗️ `align-items`

```html
<div class="d-flex align-items-center" style="height: 100px;">
    <div class="p-3 bg-primary">Alto</div>
    <div class="p-3 bg-danger h-50">Bajo</div>
</div>
```

📢 **TIP:** Usa `align-items-start` o `align-items-end` para alinear elementos en la parte superior o inferior.

### ➡️ `justify-content`

```html
<div class="d-flex justify-content-between">
    <div class="p-3 bg-info">Inicio</div>
    <div class="p-3 bg-warning">Centro</div>
    <div class="p-3 bg-danger">Final</div>
</div>
```

📢 **TIP:** Usa `justify-content-around` o `justify-content-evenly` para distribuir los elementos de manera uniforme.

---

## 🔚 Conclusión

Flexbox en Bootstrap facilita la distribución y alineación de elementos en una página sin necesidad de escribir CSS personalizado. Experimenta con estas clases y combínalas para lograr diseños responsivos y fluidos. 🚀

📌 **Recuerda:** Puedes inspeccionar elementos con DevTools (`F12`) para ver cómo afectan las clases de Bootstrap a tu diseño.
