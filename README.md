# Mustak
DAO APPLICATION 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Digital DAO Grant</title>
  <style>
    body {
      background-color: #f0f8ff;
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      padding: 50px;
    }
    .card {
      background: white;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
      display: inline-block;
      max-width: 400px;
    }
    h1 {
      color: #0066cc;
    }
    .amount {
      font-size: 24px;
      color: green;
      margin: 10px 0;
    }
    button {
      padding: 12px 24px;
      margin: 10px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }
    .accept {
      background-color: #28a745;
      color: white;
    }
    .decline {
      background-color: #dc3545;
      color: white;
    }
    .hidden {
      display: none;
    }
    .meme {
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <div class="card" id="mainCard">
    <h1>🎉 Digital DAO Grant 🎉</h1>
    <p>Congratulations! You have been selected as a Youth Tech Ambassador.</p>
    <p class="amount">Grant Approved: ৳50,00,000</p>
    <button class="accept" onclick="showPrank()">Accept</button>
    <button class="decline" onclick="alert('You declined ৳50,00,000! 😢')">Decline</button>
  </div>

  <div class="hidden" id="prankDiv">
    <h1>😂 GOTCHA!</h1>
    <p>This was a prank from your best friend! 😆</p>
    <img class="meme" src="https://i.imgur.com/6Iuj1iy.gif" alt="Prank Meme" width="300">
  </div>

  <script>
    function showPrank() {
      document.getElementById('mainCard').classList.add('hidden');
      document.getElementById('prankDiv').classList.remove('hidden');
    }
  </script>

</body>
</html>
