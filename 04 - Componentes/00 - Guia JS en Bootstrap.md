## 🏗 **Guía de JavaScript en Bootstrap**  

### 📌 Introducción  
Bootstrap no solo ofrece estilos y clases CSS, sino que también proporciona componentes interactivos que requieren **JavaScript** para funcionar. Puedes controlarlos de dos maneras:  
1. **Usando atributos `data-bs-*`** (sin escribir código JS).  
2. **Mediante la API de JavaScript de Bootstrap** (mayor control y personalización).  

---

## 🚀 **Cómo incluir Bootstrap con JavaScript**  
Para usar JavaScript en Bootstrap, necesitas incluir estos archivos en tu proyecto:  

```html
<!-- Bootstrap CSS -->
<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.css">

<!-- Bootstrap JS + Popper.js -->
<script src="./node_modules/@popperjs/core/dist/umd/popper-base.js"></script>
<script src="./node_modules/bootstrap/dist/js/bootstrap.js"></script>
```
⚠️ **Importante:** `Popper.js` es necesario para que algunos componentes como dropdowns y tooltips funcionen correctamente.

💡 **Recuerda:** Si vas a escribir código JavaScript que utilice los componentes de Bootstrap, asegúrate de colocarlo **después** de cargar `bootstrap.js`, ya que de lo contrario, las clases de Bootstrap no estarán disponibles y tu código no funcionará correctamente.  

---

## 🛠 **Uso de Bootstrap con atributos `data-bs-*`**  
Algunos componentes de Bootstrap funcionan sin necesidad de escribir código JavaScript, gracias a los atributos `data-bs-*`.  

Ejemplo de un **modal** usando solo HTML:  
```html
<!-- Botón que activa el modal -->
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#miModal">
    Abrir Modal
</button>

<!-- Modal -->
<div class="modal fade" id="miModal" tabindex="-1" aria-labelledby="miModalLabel" aria-hidden="true">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="miModalLabel">Título del Modal</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
            </div>
            <div class="modal-body">
                Contenido del modal.
            </div>
        </div>
    </div>
</div>
```
📌 **Ventaja:** Rápido y fácil de usar sin escribir JavaScript manualmente.  

---

## 🎛 **Uso de Bootstrap con JavaScript (API Bootstrap)**  
Si necesitas más control, puedes gestionar los componentes mediante JavaScript.  

### 🛠 **Ejemplo: Controlando un Modal con JavaScript**  
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modal con JavaScript</title>
    
    <link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.css">
</head>

<body>

    <!-- Botón para abrir el modal -->
    <button id="abrirModal" class="btn btn-success">Abrir Modal con JS</button>

    <!-- Modal -->
    <div class="modal fade" id="miModal" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Modal con JavaScript</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    Controlando el modal con JavaScript.
                </div>
            </div>
        </div>
    </div>

    <!-- Scripts de Bootstrap -->
    <script src="./node_modules/@popperjs/core/dist/umd/popper.min.js"></script>
    <script src="./node_modules/bootstrap/dist/js/bootstrap.js"></script>

    <script>
        // Seleccionar el modal (esto debe hacerse DESPUÉS de cargar Bootstrap.js)
        const miModal = new bootstrap.Modal(document.getElementById('miModal'));

        // Evento para abrir el modal al hacer clic en el botón
        document.getElementById('abrirModal').addEventListener('click', function () {
            miModal.show();
        });
    </script>

</body>
</html>
```
💡 **Consejo:** Siempre coloca tu código JavaScript después de `bootstrap.js`, de lo contrario, los elementos de Bootstrap no estarán disponibles aún y fallará su ejecución.

---

## 🏗 **Otros Componentes con JavaScript**  

### ✅ **Alertas dinámicas**
Puedes crear y cerrar alertas con JavaScript.  

```html
<div id="miAlerta" class="alert alert-warning alert-dismissible fade show" role="alert">
    ¡Esto es una alerta!
    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
</div>

<script>
    const alerta = new bootstrap.Alert(document.getElementById('miAlerta'));
    setTimeout(() => alerta.close(), 3000); // Cierra la alerta después de 3 segundos
</script>
```

---

### ⬇ **Dropdowns controlados con JavaScript**  
```html
<!-- Botón dropdown -->
<div class="dropdown">
    <button id="botonDropdown" class="btn btn-secondary dropdown-toggle" type="button">
        Menú desplegable
    </button>
    <ul class="dropdown-menu">
        <li><a class="dropdown-item" href="#">Opción 1</a></li>
        <li><a class="dropdown-item" href="#">Opción 2</a></li>
    </ul>
</div>

<script>
    const dropdown = new bootstrap.Dropdown(document.getElementById('botonDropdown'));
    document.getElementById('botonDropdown').addEventListener('click', () => dropdown.toggle());
</script>
```

---

## 🔥 **Tips y Consejos para Usar Bootstrap con JavaScript**  
✅ **Evita incluir múltiples veces los archivos de Bootstrap JS**, ya que puede causar errores.  
✅ **Usa `data-bs-*` siempre que puedas** para evitar escribir código innecesario.  
✅ **Usa la API JavaScript de Bootstrap** cuando necesites personalizar comportamientos.  
✅ **Si necesitas abrir/cerrar elementos dinámicamente, usa `show()`, `hide()`, `toggle()`**.  
✅ **Controla eventos con `addEventListener`** para manipular modales, alertas o dropdowns de forma dinámica.  
✅ **Siempre coloca tu código JavaScript después de `bootstrap.js` para evitar errores.**  

---
