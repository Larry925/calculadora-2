<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Calculadora para Niños</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Fredoka One', cursive;
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .calculator {
      background: #ffffffcc;
      border-radius: 30px;
      padding: 30px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.2);
      text-align: center;
    }
    .calculator h1 {
      margin-bottom: 20px;
      color: #ff4081;
    }
    input[type="number"] {
      width: 80px;
      padding: 10px;
      border: none;
      border-radius: 10px;
      margin: 10px;
      font-size: 24px;
    }
    select, button {
      font-size: 20px;
      padding: 10px;
      border-radius: 10px;
      border: none;
      margin-top: 10px;
      background-color: #ffcc80;
      color: #444;
      cursor: pointer;
    }
    button:hover {
      background-color: #ffe0b2;
    }
    .result {
      margin-top: 20px;
      font-size: 28px;
      color: #009688;
    }
  </style>
</head>
<body>
  <div class="calculator">
    <h1>🎲 Calculadora para Niños 🎲</h1>
    <input type="number" id="num1" placeholder="Número 1">
    <input type="number" id="num2" placeholder="Número 2">
    <br>
    <select id="operation">
      <option value="+">➕ Sumar</option>
      <option value="-">➖ Restar</option>
      <option value="*">✖️ Multiplicar</option>
      <option value="/">➗ Dividir</option>
    </select>
    <br>
    <button onclick="calculate()">Calcular ✅</button>
    <div class="result" id="result"></div>
  </div>

  <script>
    function calculate() {
      const num1 = parseFloat(document.getElementById("num1").value);
      const num2 = parseFloat(document.getElementById("num2").value);
      const op = document.getElementById("operation").value;
      let result = '';

      if (isNaN(num1) || isNaN(num2)) {
        result = 'Por favor ingresa dos números';
      } else {
        switch(op) {
          case '+': result = `${num1 + num2}`; break;
          case '-': result = `${num1 - num2}`; break;
          case '*': result = `${num1 * num2}`; break;
          case '/': result = num2 !== 0 ? `${num1 / num2}` : 'No se puede dividir entre 0'; break;
        }
      }

      document.getElementById("result").innerText = `Resultado: ${result}`;
    }
  </script>
</body>
</html>
