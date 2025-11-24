<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PAOLAFLIX</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Receitas Culinárias</h1>
    <p>Descubra receitas deliciosas com vídeos explicativos!</p>
  </header>

  <main>
    <div class="recipe-container">

      <!-- Bolo de Chocolate -->
      <div class="recipe-card">
        <h2>Bolo de Chocolate</h2>
        <a href="https://www.youtube.com/watch?v=7b49-fMsdd0" target="_blank" class="video-link">
          <img class="video-thumb" src="https://img.youtube.com/vi/7b49-fMsdd0/hqdefault.jpg" alt="Bolo de Chocolate">
          <div class="play-btn">▶</div>
        </a>
      </div>

      <!-- Lasanha -->
      <div class="recipe-card">
        <h2>Lasanha</h2>
        <a href="https://www.youtube.com/watch?v=2kW8hjum1zM" target="_blank" class="video-link">
          <img class="video-thumb" src="https://img.youtube.com/vi/2kW8hjum1zM/hqdefault.jpg" alt="Lasanha">
          <div class="play-btn">▶</div>
        </a>
      </div>

      <!-- Strogonoff -->
      <div class="recipe-card">
        <h2>Strogonoff</h2>
        <a href="https://www.youtube.com/watch?v=CaKY9kRhfUA" target="_blank" class="video-link">
          <img class="video-thumb" src="https://img.youtube.com/vi/CaKY9kRhfUA/hqdefault.jpg" alt="Strogonoff">
          <div class="play-btn">▶</div>
        </a>
      </div>

    </div>
  </main>

  <footer>
    
  </footer>

</body>
</html>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}

body {
  background-color: #fff8f0;
  color: #333;
}

header {
  background-color: #ff6f61;
  color: white;
  text-align: center;
  padding: 2rem 1rem;
}

header h1 {
  margin-bottom: 0.5rem;
}

.recipe-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
  padding: 2rem;
}

.recipe-card {
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  padding: 1rem;
  width: 300px;
  transition: transform 0.2s;
}

.recipe-card:hover {
  transform: scale(1.05);
}

.recipe-card h2 {
  margin: 1rem 0 0.5rem;
  color: #ff6f61;
  text-align: center;
}

.video-link {
  position: relative;
  display: block;
  width: 100%;
  height: 200px;
  cursor: pointer;
  text-decoration: none;
  border-radius: 10px;
  overflow: hidden;
}

.video-thumb {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: transform 0.3s ease;
}

.video-link:hover .video-thumb {
  transform: scale(1.05);
}

.play-btn {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 3rem;
  background-color: rgba(0, 0, 0, 0.7);
  color: #fff;
  border-radius: 50%;
  width: 70px;
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: center;
  pointer-events: none; /* deixa o clique passar para o link */
  transition: background-color 0.3s ease, transform 0.3s ease;
}

.video-link:hover .play-btn {
  background-color: rgba(255, 111, 97, 0.9);
  transform: translate(-50%, -50%) scale(1.1);
}

footer {
  text-align: center;
  padding: 1rem;
  background-color: #ff6f61;
  color: white;
  margin-top: 2rem;
}
