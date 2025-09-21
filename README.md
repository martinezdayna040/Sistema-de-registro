<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=2">
  <title>Amigo Secreto</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <main class="main-content">
    <header class="header-banner">
      <h1>Amigo Secreto</h1>
      <img src="assets/amigo-secreto.png" alt="Imagen de Amigo Secreto">
    </header>

    <form id="formAmigos" class="input-section" aria-labelledby="titulo">
      <h2 id="titulo">Agrega participantes</h2>
      <div class="input-wrapper">
        <label for="amigo" class="sr-only">Nombre del amigo</label>
        <input id="amigo" class="input-name" type="text" placeholder="Escribe un nombre" required>
        <button type="submit" class="button-add">Añadir</button>
      </div>
      <p id="mensaje" class="error-message" aria-live="assertive"></p>

      <ul id="listaAmigos" class="name-list"></ul>
      <p id="contador"></p>

      <div class="button-container">
        <button type="button" class="button-draw" onclick="sortearAmigo()"> Sortear</button>
        <button type="button" class="button-reset" onclick="reiniciar()"> Reiniciar</button>
      </div>
      <ul id="resultado" class="result-list"></ul>
    </form>
  </main>
  <script src="app.js" defer></script>
</body>
</html>
