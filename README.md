<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine?</title>
  <style>
    body {
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Segoe UI', sans-serif;
    }

    .card {
      background: white;
      padding: 30px 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
    }

    h1 {
      color: #ff4d6d;
      margin-bottom: 20px;
    }

    .buttons {
      position: relative;
      height: 60px;
    }

    button {
      padding: 10px 25px;
      font-size: 18px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: 0.2s;
    }

    #yes {
      background: #ff4d6d;
      color: white;
      margin-right: 20px;
    }

    #no {
      background: #ccc;
      position: absolute;
    }

    #message {
      margin-top: 20px;
      font-size: 22px;
      color: #ff4d6d;
      display: none;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Will you be my Valentine, Daksha? 💖</h1>

    <div class="buttons">
      <button id="yes" onclick="sayYes()">Yes</button>
      <button id="no" onmouseover="moveNo()">No</button>
    </div>

    <div id="message">
      Yayyy!! 💕🥰  
      Best Valentine ever!
    </div>
  </div>

  <script>
    function sayYes() {
      document.getElementById("message").style.display = "block";
    }

    function moveNo() {
      const noBtn = document.getElementById("no");
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 100 - 50;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    }
  </script>

</body>
</html>
