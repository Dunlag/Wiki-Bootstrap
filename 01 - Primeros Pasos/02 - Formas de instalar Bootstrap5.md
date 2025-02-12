
# Guía de Instalación de Bootstrap 5

## Opciones de Instalación

### 1. Instalación desde CDN

La forma más rápida de empezar a usar Bootstrap es agregar un enlace CDN a tu archivo HTML. Puedes incluir tanto el CSS como el JS de Bootstrap de la siguiente manera:

```html
<head>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/js/bootstrap.bundle.min.js"></script>
</body>
```

### 2. Instalación desde npm (Node Package Manager)

Instalar Bootstrap desde npm es una excelente opción si estás trabajando con un entorno de desarrollo más estructurado, ya que te permitirá actualizar las dependencias de manera sencilla y controlar las versiones de forma más eficiente.

#### Paso 1: Inicializa tu proyecto con npm

Si aún no tienes un proyecto de Node, abre tu terminal y ejecuta:

```bash
npm init -y
```

Este comando creará un archivo `package.json` para tu proyecto.

#### Paso 2: Instala Bootstrap 5

Con npm instalado, puedes instalar Bootstrap ejecutando el siguiente comando en tu terminal:

```bash
npm install bootstrap
```

Esto instalará Bootstrap 5 en tu proyecto y añadirá una entrada en el archivo `package.json` bajo las dependencias.

#### Paso 3: Agrega Bootstrap a tu HTML

Después de instalar Bootstrap, puedes referenciar los archivos CSS y JS desde la carpeta `node_modules`. En tu archivo `index.html`, usa las rutas correspondientes para incluir Bootstrap:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <!-- Enlace a Bootstrap desde Node.js -->
    <link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.css">
</head>
<body>
    <!-- Botón de Bootstrap -->
    <button class="btn btn-success">Botón</button>

    <!-- Script de Bootstrap -->
    <script src="./node_modules/bootstrap/dist/js/bootstrap.js"></script>
</body>
</html>
```

Este es un ejemplo básico que usa el archivo CSS y el archivo JS de Bootstrap desde la carpeta `node_modules`.

### 3. Instalación desde archivos descargados

Si prefieres descargar los archivos de Bootstrap directamente, puedes hacerlo desde [el sitio web de Bootstrap](https://getbootstrap.com/). Una vez descargados, solo tendrás que incluir los archivos CSS y JS en tu proyecto.

## Conclusión

La opción de instalar Bootstrap a través de npm es la más recomendable cuando estás trabajando en proyectos de desarrollo con Node.js, ya que facilita la gestión de dependencias y las actualizaciones de la biblioteca. Puedes combinar Bootstrap con herramientas como Webpack, Parcel o incluso usarlo directamente en tu archivo HTML.

¡Listo! Ahora tienes Bootstrap instalado y funcionando en tu proyecto.