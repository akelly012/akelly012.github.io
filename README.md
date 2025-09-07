# akelly012.github.io
gaming website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Play Retro Bowl</title>
  <style>
    body {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 2rem;
      background-color: #111;
      color: white;
      font-family: Arial, sans-serif;
      height: 100vh;
      margin: 0;
    }
    .play-btn {
      background-color: red;
      color: white;
      font-size: 1.5rem;
      padding: 1rem 2rem;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      transition: 0.3s;
    }
    .play-btn:hover {
      background-color: darkred;
    }
    #gameFrame {
      display: none; /* hidden until button is clicked */
      border: none;
      border-radius: 12px;
      width: 800px;
      height: 600px;
    }
  </style>
</head>
<body>
  <h1>Retro Bowl</h1>

  <!-- Red button -->
  <button class="play-btn" onclick="playRetroBowl()">Play Retro Bowl</button>

  <!-- Game iframe -->
  <iframe id="gameFrame" src="https://www.retrobowl.me/" allowfullscreen></iframe>

  <script>
    function playRetroBowl() {
      document.getElementById("gameFrame").style.display = "block";
    }
  </script>
</body>
</html>

