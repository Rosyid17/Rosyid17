<!DOCTYPE html>
<html lang="id">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pesan</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      background-color: #f5f5f5;
    }

    #hiddenMessage {
      display: none;
      font-size: 18px;
      color: #e91e63;
    }

    #showMessageBtn {
      padding: 10px;
      background-color: #e91e63;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    #showMessageBtn:hover {
      background-color: #c2185b;
    }
  </style>
</head>

<body>

  <button id="showMessageBtn" onclick="showHiddenMessage()">Pesan dari AZAM</button>

  <div id="hiddenMessage">Semogo kalian sehat selalu akhir-akhir sering hujan kalau di jalan hati-hati kalau di hati jangan pergi</div>

  <script>
    function showHiddenMessage() {
      var hiddenMessage = document.getElementById('hiddenMessage');
      var showMessageBtn = document.getElementById('showMessageBtn');

      if (hiddenMessage.style.display === 'none') {
        hiddenMessage.style.display = 'block';
        showMessageBtn.innerHTML = 'Sembunyikan Pesan';
      } else {
        hiddenMessage.style.display = 'none';
        showMessageBtn.innerHTML = 'Tampilkan Pesan Tersembunyi';
      }
    }
  </script>

</body>

</html>
