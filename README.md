# ColorKhelo<!DOCTYPE html>
<html>
<head>
  <title>Color Prediction</title>
</head>
<body>
  <h1>Predict the Color!</h1>
  <button onclick="predict('red')">Red</button>
  <button onclick="predict('green')">Green</button>
  <button onclick="predict('blue')">Blue</button>
  <h2 id="result"></h2>

  <script>
    function predict(choice) {
      const colors = ['red', 'green', 'blue'];
      const random = colors[Math.floor(Math.random() * colors.length)];

      if (choice === random) {
        document.getElementById("result").innerText = "You Won! 🎉";
      } else {
        document.getElementById("result").innerText = `You Lost! Color was ${random}`;
      }
    }
  </script>
</body>
</html>
