# HTML
html
<!DOCTYPE html>
<html lang="ca">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pàgina responsive d'exemple</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #004466;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      background-color: #006699;
      display: flex;
      justify-content: center;
      gap: 20px;
      padding: 10px;
      flex-wrap: wrap; /* fa que en pantalles xicotetes els enllaços baixen */
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    main {
      padding: 20px;
    }

    h2 {
      border-bottom: 2px solid #004466;
      padding-bottom: 5px;
    }

    table {
      border-collapse: collapse;
      width: 100%;
      margin: 20px 0;
    }

    table, th, td {
      border: 1px solid #004466;
    }

    th, td {
      padding: 10px;
      text-align: center;
    }

    th {
      background-color: #006699;
      color: white;
    }

    form {
      margin-top: 20px;
      padding: 15px;
      border: 1px solid #ccc;
      border-radius: 8px;
      background-color: #f5f5f5;
      max-width: 100%;
    }

    label {
      display: block;
      margin-top: 10px;
      font-weight: bold;
    }

    input, textarea, button {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border-radius: 5px;
      border: 1px solid #ccc;
      font-size: 14px;
    }

    button {
      background-color: #004466;
      color: white;
      font-weight: bold;
      cursor: pointer;
      margin-top: 15px;
    }

    button:hover {
      background-color: #006699;
    }

    footer {
      background-color: #004466;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 20px;
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      nav {
        flex-direction: column;
        align-items: center;
      }

      table, th, td {
        font-size: 14px;
      }

      main {
        padding: 10px;
      }
    }

    @media (max-width: 480px) {
      header h1 {
        font-size: 22px;
      }

      nav a {
        font-size: 14px;
      }

      table, th, td {
        font-size: 12px;
      }

      button {
        font-size: 14px;
        padding: 10px;
      }
    }
  </style>
</head>
<body>
  <!-- Capçalera -->
  <header>
    <h1>Benvinguts a la meua pàgina web</h1>
    <p>Versió responsive amb HTML i CSS</p>
  </header>

  <!-- Menú de navegació -->
  <nav>
    <a href="#">Inici</a>
    <a href="#">Sobre mi</a>
    <a href="#">Projectes</a>
    <a href="#">Contacte</a>
  </nav>

  <!-- Contingut principal -->
  <main>
    <h2>Secció principal</h2>
    <p>Aquesta és la secció principal de la pàgina. Pots afegir text, imatges, llistes, taules i formularis.</p>

    <h3>Llista d’exemple:</h3>
    <ul>
      <li>Element 1</li>
      <li>Element 2</li>
      <li>Element 3</li>
    </ul>

    <h3>Taula d’exemple:</h3>
    <table>
      <tr>
        <th>Nom</th>
        <th>Edat</th>
        <th>Ciutat</th>
      </tr>
      <tr>
        <td>Maria</td>
        <td>25</td>
        <td>València</td>
      </tr>
      <tr>
        <td>Joan</td>
        <td>30</td>
        <td>Castelló</td>
      </tr>
      <tr>
        <td>Laura</td>
        <td>28</td>
        <td>Alacant</td>
      </tr>
    </table>

    <h3>Formulari de contacte:</h3>
    <form>
      <label for="nom">Nom:</label>
      <input type="text" id="nom" name="nom" required>

      <label for="email">Correu electrònic:</label>
      <input type="email" id="email" name="email" required>

      <label for="missatge">Missatge:</label>
      <textarea id="missatge" name="missatge" rows="5" required></textarea>

      <button type="submit">Enviar</button>
    </form>
  </main>

  <!-- Peu de pàgina -->
  <footer>
    <p>&copy; 2025 — Pàgina d'exemple responsive creada en HTML i CSS</p>
  </footer>
</body>
</html>
