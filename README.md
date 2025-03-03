# challeng-amigo-secreto
# Amigo Secreto

El principal objetivo de este desafío es fortalecer tus habilidades en lógica de programación. Aquí deberás desarrollar la lógica para resolver el problema de un sorteo de amigo secreto.

## Descripción

Este proyecto permite a los usuarios agregar nombres a una lista de amigos y luego sortear un amigo secreto de manera aleatoria. La aplicación está construida utilizando HTML, CSS y JavaScript.

## Funcionalidades

- **Agregar Amigo**: Permite al usuario ingresar un nombre en el campo de texto y añadirlo a la lista de amigos.
- **Sortear Amigo**: Selecciona de manera aleatoria uno de los nombres almacenados en el array de amigos y muestra el resultado.

## Estructura del Proyecto

- `index.html`: Contiene la estructura HTML de la aplicación.
- `style.css`: Contiene los estilos CSS para la aplicación.
- `app.js`: Contiene la lógica de la aplicación en JavaScript.

## Instrucciones

### Agregar Amigo

1. Ingrese el nombre de un amigo en el campo de texto.
2. Haga clic en el botón "Añadir".
3. El nombre se añadirá a la lista de amigos y el campo de texto se limpiará automáticamente.

### Sortear Amigo

1. Asegúrese de que haya al menos un nombre en la lista de amigos.
2. Haga clic en el botón "Sortear amigo".
3. Un nombre será seleccionado de manera aleatoria y se mostrará en la sección de resultados.



## Código

### HTML

##### html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100;400;700;900&family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&display=swap" rel="stylesheet">
    <title>Amigo Secreto</title>
</head>
<body>
    <main class="main-content">
        <header class="header-banner">
            <h1 class="main-title">Amigo Secreto</h1>
            <img src="assets/amigo-secreto.png" alt="Imagen representativa de amigo secreto">
        </header>
        
        <section class="input-section">
            <h2 class="section-title">Digite el nombre de sus amigos</h2>
            <div class="input-wrapper">
                <input type="text" id="amigo" class="input-name" placeholder="Escribe un nombre">
                <button class="button-add" onclick="agregarAmigo()">Añadir</button>
            </div>
           
            <ul id="listaAmigos" class="name-list" aria-labelledby="listaAmigos" role="list"></ul>
            <ul id="resultado" class="result-list" aria-live="polite"></ul>

            <div class="button-container">
                <button class="button-draw" onclick="sortearAmigo()" aria-label="Sortear amigo secreto">
                    <img src="assets/play_circle_outline.png" alt="Ícono para sortear">
                    Sortear amigo
                </button>
            </div>
        </section>
    </main>

    <script src="app.js" defer></script>
</body>
</html>


## Créditos

Este proyecto fue desarrollado como parte de un desafío para fortalecer habilidades en lógica de programación.

## Licencia
Este proyecto está bajo la Licencia MIT.