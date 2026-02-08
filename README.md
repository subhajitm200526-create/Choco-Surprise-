for kissmiss
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chocolate Surprise</title>
<style>
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    height: 100vh;
    background: #ffe6e6;
    font-family: Arial, sans-serif;
  }
  #gift {
    width: 200px;
    height: 200px;
    background: #ff3366;
    border-radius: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 28px;
    cursor: pointer;
    text-align: center;
    transition: transform 0.5s;
  }
  #gift:hover {
    transform: scale(1.1);
  }
  #chocolates {
    display: none;
    margin-top: 20px;
    text-align: center;
    font-size: 50px;
  }
  .choco {
    display: inline-block;
    margin: 10px;
    animation: float 2s infinite alternate;
  }
  @keyframes float {
    0% { transform: translateY(0px); }
    100% { transform: translateY(-20px); }
  }
  h2 {
    margin-top: 20px;
    color: #800000;
    text-shadow: 1px 1px 2px #fff;
  }
</style>
</head>
<body>

<div id="gift">🎁 Tap to Open!</div>

<div id="chocolates">
  <span class="choco">🍫</span>
  <span class="choco">🍫</span>
  <span class="choco">🍫</span>
  <h2>Happy Chocolate Day Kissmiss! ❤️</h2>
</div>

<script>
  const gift = document.getElementById('gift');
  const chocolates = document.getElementById('chocolates');

  gift.addEventListener('click', () => {
    gift.style.display = 'none';
    chocolates.style.display = 'block';
  });
</script>

</body>
</html>
