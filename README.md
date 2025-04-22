<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Film - UpdateMovie121</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #121212;
      color: #f1f1f1;
      padding: 20px;
    }
    .container {
      max-width: 800px;
      margin: auto;
    }
    .poster {
      width: 100%;
      border-radius: 10px;
    }
    h1 {
      margin-top: 20px;
    }
    .watch-button {
      display: inline-block;
      margin-top: 20px;
      padding: 12px 24px;
      background-color: #e50914;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      transition: background 0.3s ease;
    }
    .watch-button:hover {
      background-color: #b0060f;
    }
    .description {
      margin-top: 20px;
      line-height: 1.6;
    }
  </style>
</head>
<body>
  <div class="container">
    <img class="poster" id="poster" src="" alt="Poster Film">
    <h1 id="judul">Judul Film</h1>
    <p class="description" id="sinopsis">Sinopsis akan ditampilkan di sini.</p>
    <a href="#" target="_blank" class="watch-button" id="watchLink">Nonton Sekarang</a>
  </div>

  <script>
    const urlParams = new URLSearchParams(window.location.search);
    const id = urlParams.get("id");

    const dataFilm = {
      "matrix": {
        "judul": "The Matrix",
        "gambar": "https://via.placeholder.com/800x450?text=The+Matrix",
        "sinopsis": "Seorang hacker menemukan kenyataan bahwa dunia adalah simulasi.",
        "link": "https://www.profitableratecpm.com/suqgszz3kg?key=fe9492f367b3cc5b77c15cff87bdebf9"
      },
      "inception": {
        "judul": "Inception",
        "gambar": "https://via.placeholder.com/800x450?text=Inception",
        "sinopsis": "Seorang pencuri masuk ke mimpi untuk mencuri rahasia.",
        "link": "https://www.profitableratecpm.com/suqgszz3kg?key=fe9492f367b3cc5b77c15cff87bdebf9"
      }
    };

    const film = dataFilm[id];

    if (film) {
      document.title = film.judul + " - UpdateMovie121";
      document.getElementById("judul").textContent = film.judul;
      document.getElementById("poster").src = film.gambar;
      document.getElementById("sinopsis").textContent = film.sinopsis;
      document.getElementById("watchLink").href = film.link;
    } else {
      document.getElementById("judul").textContent = "Film tidak ditemukan";
      document.getElementById("poster").style.display = "none";
      document.getElementById("watchLink").style.display = "none";
    }
  </script>

  <script type='text/javascript' src='//pl24641220.profitableratecpm.com/d7/e9/46/d7e946432742510fceeead077a3e8394.js'></script>
</body>
</html>
