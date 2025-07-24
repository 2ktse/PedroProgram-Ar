<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Smart Predictor Tool</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }
    body {
      background: linear-gradient(to bottom, #000000, #1c1c1c);
      color: white;
      text-align: center;
      padding: 20px;
    }
    header {
      margin-bottom: 30px;
    }
    header h1 {
      font-size: 2em;
      margin-bottom: 10px;
    }
    .platform-buttons button {
      margin: 10px;
      padding: 15px 25px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      background-color: #ff3c00;
      color: white;
    }
    .input-section {
      margin: 40px 0;
    }
    .input-section input {
      padding: 10px;
      width: 80%;
      max-width: 300px;
      border-radius: 6px;
      border: none;
      margin-bottom: 20px;
    }
    .input-section button {
      padding: 10px 25px;
      border: none;
      background: #00c853;
      color: white;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
    }
    footer {
      margin-top: 60px;
      font-size: 14px;
      color: #aaa;
    }
  </style>
</head>
<body>
  <header>
    <h1>Smart Predictor Tool</h1>
    <p>Unlock smart predictions for your bets!</p>
  </header>

  <div class="platform-buttons">
    <button onclick="selectPlatform('1xbet')">1xBet</button>
    <button onclick="selectPlatform('betwinner')">Betwinner</button>
  </div>

  <div class="input-section">
    <input type="text" id="userId" placeholder="Enter your ID">
    <br>
    <button onclick="submitId()">Activate Tool</button>
  </div>

  <footer>
    <p>&copy; 2025 Predictor Tool. All rights reserved.</p>
  </footer>

  <script>
    function selectPlatform(name) {
      alert("Selected platform: " + name);
    }

    function submitId() {
      const id = document.getElementById('userId').value;
      if (!id) {
        alert("Please enter your ID");
        return;
      }
      alert("Tool activated for ID: " + id);
      // You can redirect or send data here
    }
  </script>
</body>
</html>
