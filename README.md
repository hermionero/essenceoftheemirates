<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Essence of the Emirates</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <h1>Essence of the Emirates</h1>
  <p>Explore a world where tradition meets tomorrow.</p>
</header>

<section id="hero">
  <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=1400&q=80" alt="Desert and Skyline">
</section>

<section id="cultural-creatures">
  <h2>Guardians of the Land</h2>
  <div class="carousel">
    <img src="https://images.unsplash.com/photo-1554059208-3237f6d596af?auto=format&fit=crop&w=800&q=80" alt="Camel">
    <img src="https://images.unsplash.com/photo-1589047133271-9414be5e650f?auto=format&fit=crop&w=800&q=80" alt="Gazelle">
    <img src="https://images.unsplash.com/photo-1583947582880-40c6a0d08aa0?auto=format&fit=crop&w=800&q=80" alt="Falcon">
  </div>
</section>

<section id="architecture">
  <h2>Built with Identity</h2>
  <div class="architecture-container">
    <img src="https://images.unsplash.com/photo-1605902711622-cfb43c4437a7?auto=format&fit=crop&w=800&q=80" alt="Heritage Fort">
    <img src="https://images.unsplash.com/photo-1526747709897-646d8e3e8f9a?auto=format&fit=crop&w=800&q=80" alt="Modern Skyline">
  </div>
</section>

<section id="environments">
  <h2>Environments of the Emirates</h2>
  <div class="gallery">
    <img src="https://images.unsplash.com/photo-1617306497405-0e7a5ec1480a?auto=format&fit=crop&w=800&q=80" alt="Pearl Diving">
    <img src="https://images.unsplash.com/photo-1585647340928-8944b54800a5?auto=format&fit=crop&w=800&q=80" alt="Desert Oasis">
    <img src="https://images.unsplash.com/photo-1580841144262-630bae14ed97?auto=format&fit=crop&w=800&q=80" alt="Souk">
  </div>
</section>

<section id="calligraphy">
  <h2>Arabic Calligraphy</h2>
  <p>Drag and interact with beautiful Arabic script in the modern world!</p>
</section>

<footer>
  <p>Created to honor the spirit of the Emirates. 🇴🇲</p>
</footer>

<script src="script.js"></script>
</body>
</html>
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  background-color: #fdf6ec;
  color: #333;
}

header {
  background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1585241936938-5cbd8d0ffb2e?auto=format&fit=crop&w=1400&q=80') center/cover;
  color: white;
  padding: 60px 20px;
  text-align: center;
}

#hero img {
  width: 100%;
  height: auto;
  display: block;
}

section {
  padding: 40px 20px;
  text-align: center;
}

.carousel img, .architecture-container img, .gallery img {
  width: 250px;
  height: 180px;
  margin: 10px;
  border-radius: 15px;
  transition: transform 0.3s;
}

.carousel img:hover, .architecture-container img:hover, .gallery img:hover {
  transform: scale(1.1);
}

footer {
  background-color: #222;
  color: white;
  padding: 20px;
  text-align: center;
}

h1, h2 {
  font-family: 'Amiri', serif;
}
// Basic animation or effects can go here if needed
document.querySelectorAll('.carousel img').forEach((img) => {
  img.addEventListener('mouseover', () => {
    img.style.transform = 'scale(1.2)';
  });
  img.addEventListener('mouseout', () => {
    img.style.transform = 'scale(1)';
  });
});

// You can add more animations for future expansion!
