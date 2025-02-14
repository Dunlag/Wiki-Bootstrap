# Guía de Grid en Bootstrap

El sistema de Grid de Bootstrap permite crear diseños flexibles y responsivos de manera sencilla. Se basa en un sistema de filas y columnas que facilita la distribución del contenido.

## 📌 Conceptos clave
- **Contenedor (`.container`, `.container-fluid`)**: Define los límites del grid.
- **Filas (`.row`)**: Agrupan columnas dentro de un contenedor.
- **Columnas (`.col`, `.col-*`)**: Dividen el espacio dentro de una fila.
- **Breakpoints (`col-sm-*`, `col-md-*`, `col-lg-*`, `col-xl-*`)**: Permiten diseños adaptativos en diferentes tamaños de pantalla.

## 🏗️ Ejemplos de Grid

### 🔹 Ejemplo básico
```html
<div class="row text-white">
    <div class="col bg-primary p-3">Columna 1</div>
    <div class="col bg-danger p-3">Columna 2</div>
    <div class="col bg-primary p-3">Columna 3</div>
</div>
```
💡 **Consejo:** Si no defines el tamaño de las columnas, Bootstrap las distribuirá equitativamente.

---

### 🔹 Especificando tamaños de columna
```html
<div class="row text-white">
    <div class="col-4 bg-success p-3">Col 4</div>
    <div class="col-8 bg-warning p-3">Col 8</div>
</div>
```
💡 **Tip:** La suma de los valores debe ser 12 para mantener una fila completa.

---

### 🔹 Distribución y alineación
```html
<div class="row justify-content-between text-white">
    <div class="col-3 bg-info p-3">Izquierda</div>
    <div class="col-3 bg-secondary p-3">Centro</div>
    <div class="col-3 bg-dark p-3">Derecha</div>
</div>
```
💡 **Tip:** Usa `justify-content-start`, `justify-content-center` o `justify-content-end` para alinear elementos horizontalmente.

---

### 🔹 Anidación de columnas
```html
<div class="row text-white">
    <div class="col bg-primary p-3">
        Columna principal
        <div class="row mt-2">
            <div class="col bg-light text-dark p-2">Subcolumna 1</div>
            <div class="col bg-light text-dark p-2">Subcolumna 2</div>
        </div>
    </div>
</div>
```
💡 **Consejo:** Puedes anidar columnas dentro de otra columna para crear estructuras más complejas.

---

### 🔹 Columnas con diferentes alturas
```html
<div class="row align-items-end text-white" style="height: 200px;">
    <div class="col bg-success p-3">Baja</div>
    <div class="col bg-danger p-5">Alta</div>
    <div class="col bg-info p-2">Más baja</div>
</div>
```
💡 **Tip:** Usa `align-items-start`, `align-items-center` o `align-items-end` para controlar la alineación vertical.

## 🎯 Consejos generales
✅ Usa clases de utilidad (`g-3`, `p-3`, `m-2`) para mejorar el espaciado.  
✅ Recuerda que Bootstrap usa un sistema de 12 columnas, pero puedes combinar tamaños.  
✅ Aplica `order-*` para cambiar el orden de las columnas sin modificar el HTML.  
✅ Usa `col-auto` si quieres que una columna solo ocupe el espacio de su contenido.  

---

Este sistema de Grid te ayudará a crear diseños modernos y flexibles. 🚀 ¡Experimenta con Bootstrap y sácale el máximo partido! 💡

