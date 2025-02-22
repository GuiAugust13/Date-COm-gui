<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Escolha o Restaurante</title>
  <style>
    body { font-family: Arial, sans-serif; text-align: center; padding: 20px; }
    button { margin: 10px; padding: 15px 30px; font-size: 16px; border-radius: 10px; border: none; background-color: #4CAF50; color: white; cursor: pointer; }
    button:hover { background-color: #45a049; }
  </style>
</head>
<body>
  <h1>Escolha um número de 1 a 5</h1>
  <div id="buttons">
    <button onclick="chooseOption(1)">1</button>
    <button onclick="chooseOption(2)">2</button>
    <button onclick="chooseOption(3)">3</button>
    <button onclick="chooseOption(4)">4</button>
    <button onclick="chooseOption(5)">5</button>
  </div>

  <script>
    function chooseOption(number) {
      const restaurants = {
        1: { name: "Lellis Trattoria - Curitiba", link: "https://goo.gl/maps/GXyaH9nYQ2c3QjKg8" },
        2: { name: "Ernesto Ristorante", link: "https://goo.gl/maps/KURXbhBWSy52" },
        3: { name: "Armazém Dom Carmino Pizzaria", link: "https://goo.gl/maps/J7N5WaHE8jQ2" },
        4: { name: "Restaurante Scavollo", link: "https://goo.gl/maps/zUMT8vLq5nL2" },
        5: { name: "Italy Caffé Champagnat", link: "https://goo.gl/maps/QFVZkLw2iPR2" }
      };
      const choice = restaurants[number];
      if (choice) {
        alert(`Voc\u00ea escolheu: ${choice.name}`);
        window.location.href = choice.link;
      }
    }
  </script>
</body>
</html>
