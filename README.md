# MilanoUp
<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Info Milano - Servizi Gratuiti</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <div class="logo">InfoMilano</div>
      <ul class="nav-links">
        <li><a href="#servizi">Servizi</a></li>
        <li><a href="#video">Video</a></li>
        <li><a href="#contatti">Contatti</a></li>
      </ul>
    </nav>
    <div class="hero">
      <h1>Scopri Milano con noi</h1>
      <p>Offriamo informazioni gratuite su trasporti, eventi, luoghi da visitare e altro!</p>
      <a href="#servizi" class="btn">Esplora i Servizi</a>
    </div>
  </header>

  <main>
    <section id="servizi" class="servizi">
      <h2>Cosa Offriamo</h2>
      <div class="cards">
        <div class="card">
          <img src="https://source.unsplash.com/400x200/?milan,duomo" alt="Duomo di Milano">
          <h3>Luoghi da visitare</h3>
          <p>Scopri monumenti e attrazioni imperdibili a Milano.</p>
        </div>
        <div class="card">
          <img src="https://source.unsplash.com/400x200/?tram,milan" alt="Trasporti">
          <h3>Trasporti</h3>
          <p>Orari, biglietti e come muoversi comodamente.</p>
        </div>
        <div class="card">
          <img src="https://source.unsplash.com/400x200/?event,concert" alt="Eventi">
          <h3>Eventi</h3>
          <p>Concerti, mostre, festival e attività settimanali.</p>
        </div>
      </div>
    </section>

    <section id="video" class="video-section">
      <h2>Scopri Milano in Video</h2>
      <iframe width="100%" height="400" src="https://www.youtube.com/embed/GwOjpQGv5l8" title="Milano Video" frameborder="0" allowfullscreen></iframe>
    </section>

    <section class="gif-section">
      <h2>Un Tocco Divertente</h2>
      <img src="https://media.giphy.com/media/3o7aCSPqXE5C6T8tBC/giphy.gif" alt="Milano GIF" class="gif">
    </section>
  </main>

  <footer id="contatti">
    <h2>Contattaci</h2>
    <p>Email: info@milano-gratis.it</p>
    <p>Instagram: <a href="https://instagram.com/infomilano">@infomilano</a></p>
    <p>&copy; 2025 InfoMilano. Tutti i diritti riservati.</p>
  </footer>
</body>
</html>
from zipfile import ZipFile
from pathlib import Path

# Creazione dei contenuti HTML e CSS
html_content = """<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Info Milano - Servizi Gratuiti</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <div class="logo">InfoMilano</div>
      <ul class="nav-links">
        <li><a href="#servizi">Servizi</a></li>
        <li><a href="#video">Video</a></li>
        <li><a href="#contatti">Contatti</a></li>
      </ul>
    </nav>
    <div class="hero">
      <h1>Scopri Milano con noi</h1>
      <p>Offriamo informazioni gratuite su trasporti, eventi, luoghi da visitare e altro!</p>
      <a href="#servizi" class="btn">Esplora i Servizi</a>
    </div>
  </header>

  <main>
    <section id="servizi" class="servizi">
      <h2>Cosa Offriamo</h2>
      <div class="cards">
        <div class="card">
          <img src="https://source.unsplash.com/400x200/?milan,duomo" alt="Duomo di Milano">
          <h3>Luoghi da visitare</h3>
          <p>Scopri monumenti e attrazioni imperdibili a Milano.</p>
        </div>
        <div class="card">
          <img src="https://source.unsplash.com/400x200/?tram,milan" alt="Trasporti">
          <h3>Trasporti</h3>
          <p>Orari, biglietti e come muoversi comodamente.</p>
        </div>
        <div class="card">
          <img src="https://source.unsplash.com/400x200/?event,concert" alt="Eventi">
          <h3>Eventi</h3>
          <p>Concerti, mostre, festival e attività settimanali.</p>
        </div>
      </div>
    </section>

    <section id="video" class="video-section">
      <h2>Scopri Milano in Video</h2>
      <iframe width="100%" height="400" src="https://www.youtube.com/embed/GwOjpQGv5l8" title="Milano Video" frameborder="0" allowfullscreen></iframe>
    </section>

    <section class="gif-section">
      <h2>Un Tocco Divertente</h2>
      <img src="https://media.giphy.com/media/3o7aCSPqXE5C6T8tBC/giphy.gif" alt="Milano GIF" class="gif">
    </section>
  </main>

  <footer id="contatti">
    <h2>Contattaci</h2>
    <p>Email: info@milano-gratis.it</p>
    <p>Instagram: <a href="https://instagram.com/infomilano">@infomilano</a></p>
    <p>&copy; 2025 InfoMilano. Tutti i diritti riservati.</p>
  </footer>
</body>
</html>
"""

css_content = """/* style.css */
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background-color: #f7f9fc;
  color: #333;
  line-height: 1.6;
}

header {
  background: linear-gradient(to right, #0066ff, #00ccff);
  color: white;
  padding-bottom: 3rem;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

.hero {
  text-align: center;
  padding: 3rem 1rem;
}

.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.hero .btn {
  display: inline-block;
  background: white;
  color: #0066ff;
  padding: 0.8rem 1.5rem;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
  margin-top: 1rem;
}

.servizi {
  padding: 3rem 2rem;
  text-align: center;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
  margin-top: 2rem;
}

.card {
  background: white;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  padding: 1rem;
  width: 300px;
}

.card img {
  max-width: 100%;
  border-radius: 10px;
}

.video-section, .gif-section {
  padding: 3rem 2rem;
  text-align: center;
}

.gif {
  width: 300px;
  border-radius: 10px;
}

footer {
  background: #222;
  color: white;
  text-align: center;
  padding: 2rem;
}

footer a {
  color: #00ccff;
  text-decoration: none;
}
"""

# Salvataggio file temporanei
base_path = Path("/mnt/data/info-milano")
base_path.mkdir(parents=True, exist_ok=True)

html_path = base_path / "index.html"
css_path = base_path / "style.css"

html_path.write_text(html_content, encoding="utf-8")
css_path.write_text(css_content, encoding="utf-8")

# Creazione dello ZIP
zip_path = Path("/mnt/data/info-milano.zip")
with ZipFile(zip_path, 'w') as zipf:
    zipf.write(html_path, arcname="index.html")
    zipf.write(css_path, arcname="style.css")

zip_path.name  # Nome del file zip creato per download

