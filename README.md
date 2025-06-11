<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Confess Untukmu</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: 'Arial', sans-serif;
      background: #fff0f6;
      color: #880e4f;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }
    .container {
      text-align: center;
      padding: 40px;
    }
    .fade {
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }
    .fade.show {
      opacity: 1;
    }
    .confess-box {
      font-size: 24px;
      background: #fff;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      max-width: 500px;
      margin: auto;
    }
    .button {
      background: #f06292;
      color: white;
      padding: 12px 24px;
      margin-top: 20px;
      border: none;
      border-radius: 10px;
      font-size: 18px;
      cursor: pointer;
      transition: background 0.3s;
    }
    .button:hover {
      background: #ec407a;
    }
    #closing {
      font-size: 22px;
      margin-top: 20px;
      color: #4a148c;
    }
  </style>
</head>
<body>
  <div class="container">
    <div id="opening" class="confess-box fade show">
      Hai... sebelum kamu lanjut, aku mau ngomong sesuatu 😳
      <br><br>
      <button class="button" onclick="showConfess()">Lanjut 👉</button>
    </div>

    <div id="confess" class="confess-box fade">
      Aku udah lama ngerasa ini... dan aku nggak bisa diem aja lagi.
      <br><br>
      Aku suka kamu. Beneran. Dari hati ❤️
      <br><br>
      <button class="button" onclick="showClosing()">🥺</button>
    </div>

    <div id="closing" class="fade">
      Makasih udah baca sampai sini... apa pun jawabannya, kamu tetap spesial ✨
    </div>
  </div>

  <script>
    function showConfess() {
      document.getElementById('opening').classList.remove('show');
      document.getElementById('confess').classList.add('show');
    }
    function showClosing() {
      document.getElementById('confess').classList.remove('show');
      document.getElementById('closing').classList.add('show');
    }
  </script>
</body>
</html>
