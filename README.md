# chemistry-formulas
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chemistry Formulas</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f9;
      color: #333;
      text-align: center;
      padding: 20px;
    }
    .container {
      max-width: 600px;
      margin: 0 auto;
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0px 4px 6px rgba(0,0,0,0.1);
    }
    h1 {
      color: #5a67d8;
    }
    input, button {
      padding: 10px;
      margin: 5px;
      border: 1px solid #ddd;
      border-radius: 5px;
      font-size: 16px;
    }
    button {
      background-color: #5a67d8;
      color: white;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Chemistry Formulas Calculator</h1>

    <!-- Moles to Grams -->
    <h3>Moles to Grams Conversion</h3>
    <input type="number" id="moles" placeholder="Enter moles" />
    <input type="number" id="molarMass" placeholder="Enter molar mass (g/mol)" />
    <button onclick="convertMolesToGrams()">Calculate</button>
    <p id="gramsResult"></p>

    <script>
      function convertMolesToGrams() {
        const moles = parseFloat(document.getElementById('moles').value);
        const molarMass = parseFloat(document.getElementById('molarMass').value);
        const result = moles * molarMass;
        document.getElementById('gramsResult').innerText = `Mass = ${result} g`;
      }
    </script>
  </div>
</body>
</html>
