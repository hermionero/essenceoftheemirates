<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Essence of the Emirates</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      overflow-x: hidden;
      font-family: 'Poppins', sans-serif;
      background-color: #f9f9f9;
    }
    /* Hero Section */
    .hero {
      position: relative;
      width: 100%;
      height: 100vh;
      display: flex;
    }
    .hero-left, .hero-right {
      flex: 1;
      height: 100%;
    }
    .hero-left {
      background: url('https://images.unsplash.com/photo-1617110466240-fb812d1cc34e') center/cover no-repeat;
    }
    .hero-right {
      background: url('https://images.unsplash.com/photo-1549917304-5f20d1b4b4cf') center/cover no-repeat;
    }
    .hero-text {
      position: absolute;
      top: 40%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      color: white;
      text-shadow: 2px 2px 4px #000;
    }
    .hero-text h1 {
      font-size: 3rem;
    }
    .hero-text button {
      margin-top: 20px;
      padding: 12px 24px;
      background-color: #FFD700;
      border: none;
      border-radius: 30px;
      font-size: 1rem;
      cursor: pointer;
      box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
    }
    /* Falcon Animation */
    .falcon {
      position: absolute;
      width: 100px;
      top: 20%;
      left: -150px;
      animation: fly 10s linear infinite;
    }
    @keyframes fly {
      0% { left: -150px; top: 20%; }
      50% { left: 50%; top: 10%; }
      100% { left: 110%; top: 20%; }
    }

    /* Animal Carousel Section */
    .carousel-section {
      padding: 60px 20px;
      text-align: center;
      background: #ffffff;
    }
    .carousel-section h2 {
      font-size: 2.5rem;
      margin-bottom: 40px;
      color: #333;
    }
    .carousel-container {
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
    }
    .animal-card {
      background: #f0e68c;
      border-radius: 20px;
      width: 220px;
      padding: 20px;
      transition: transform 0.3s, background 0.3s;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    .animal-card img {
      width: 100px;
      height: 100px;
    }
    .animal-card h3 {
      margin-top: 15px;
      font-size: 1.5rem;
    }
    .animal-card p {
      font-size: 1rem;
      color: #555;
      margin-top: 10px;
      display: none;
    }
    .animal-card:hover {
      background: #ffeb99;
      transform: scale(1.05);
    }
    .animal-card:hover p {
      display: block;
    }
  </style>
</head>

<body>

<!-- Hero Section -->
<div class="hero">
  <div class="hero-left"></div>
  <div class="hero-right"></div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Falcon_flying.png" class="falcon" alt="Falcon">
  <div class="hero-text">
    <h1>Welcome to the Spirit of the Emirates</h1>
    <button>Explore More</button>
  </div>
</div>

<!-- Animal Carousel Section -->
<div class="carousel-section">
  <h2>Guardians of the Land</h2>
  <div class="carousel-container">
    
    <div class="animal-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/6/69/Dromedary_in_the_desert.jpg" alt="Camel">
      <h3>Camel</h3>
      <p>Symbol of endurance and resilience in the desert.</p>
    </div>

    <div class="animal-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/7/7c/Gazelle_Nanyuki.jpg" alt="Gazelle">
      <h3>Gazelle</h3>
      <p>Symbol of grace, beauty, and speed.</p>
    </div>

    <div class="animal-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Falcon_flying.png" alt="Falcon">
      <h3>Falcon</h3>
      <p>Symbol of power, vision, and leadership.</p>
    </div>

  </div>
</div>

</body>
</html>
<!-- Architecture Inspirations Section -->
<div class="architecture-section">
  <h2>Built with Identity</h2>
  <div class="architecture-container">
    
    <!-- Traditional Architecture -->
    <div class="architecture-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/f/fd/Al_Fahidi_Fort_Dubai_2007.jpg" alt="Traditional Fort">
      <div class="architecture-text">
        <h3>Traditional Forts & Wind Towers</h3>
        <p>Symbols of protection, ventilation, and community life.</p>
      </div>
    </div>

    <!-- Modern Architecture -->
    <div class="architecture-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/9/9e/Burj_Khalifa.jpg" alt="Burj Khalifa">
      <div class="architecture-text">
        <h3>Modern Marvels</h3>
        <p>Burj Khalifa and Louvre Abu Dhabi — icons of ambition and innovation.</p>
      </div>
    </div>

  </div>
</div>

<!-- Add this style inside <style> tag -->
<style>
/* Architecture Section */
.architecture-section {
  padding: 60px 20px;
  background: #f2f2f2;
  text-align: center;
}
.architecture-section h2 {
  font-size: 2.5rem;
  margin-bottom: 40px;
  color: #222;
}
.architecture-container {
  display: flex;
  justify-content: center;
  gap: 40px;
  flex-wrap: wrap;
}
.architecture-card {
  position: relative;
  width: 320px;
  height: 400px;
  overflow: hidden;
  border-radius: 20px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.2);
  cursor: pointer;
  transition: transform 0.4s;
  background-color: white;
}
.architecture-card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.4s;
}
.architecture-card:hover img {
  transform: scale(1.1);
}
.architecture-text {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 20px;
  background: rgba(0, 0, 0, 0.6);
  color: white;
  opacity: 0;
  transition: opacity 0.4s;
}
.architecture-card:hover .architecture-text {
  opacity: 1;
}
.architecture-text h3 {
  font-size: 1.5rem;
}
.architecture-text p {
  font-size: 1rem;
  margin-top: 10px;
}
</style>
<!-- Environments of the Emirates Section -->
<div class="environments-section">
  <h2>Environments of the Emirates</h2>
  <div class="environments-gallery">
    
    <!-- Desert -->
    <div class="environment-card" style="background-image: url('https://images.unsplash.com/photo-1590595905515-11b6d20d9025');">
      <div class="environment-text">
        <h3>Desert Dunes</h3>
        <p>Endless sands tell stories of endurance and mystery.</p>
      </div>
    </div>

    <!-- Oasis -->
    <div class="environment-card" style="background-image: url('https://images.unsplash.com/photo-1582142401955-b7045ed40a68');">
      <div class="environment-text">
        <h3>Oases</h3>
        <p>Life blooms where water whispers in the desert.</p>
      </div>
    </div>

    <!-- Maritime -->
    <div class="environment-card" style="background-image: url('https://images.unsplash.com/photo-1613667769827-c58fbba7edb5');">
      <div class="environment-text">
        <h3>Maritime Heritage</h3>
        <p>Seafaring and pearl diving shaped coastal traditions.</p>
      </div>
    </div>

    <!-- Souks -->
    <div class="environment-card" style="background-image: url('https://images.unsplash.com/photo-1578589318432-5ef80a6268dd');">
      <div class="environment-text">
        <h3>Traditional Souks</h3>
        <p>Markets full of colors, aromas, and lively trade.</p>
      </div>
    </div>

    <!-- Modern Skylines -->
    <div class="environment-card" style="background-image: url('https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0');">
      <div class="environment-text">
        <h3>Modern Skylines</h3>
        <p>Ambitious cities rising into tomorrow's dreams.</p>
      </div>
    </div>

  </div>
</div>

<!-- Add this style inside <style> tag -->
<style>
/* Environments Section */
.environments-section {
  padding: 60px 20px;
  background: #ffffff;
  text-align: center;
}
.environments-section h2 {
  font-size: 2.5rem;
  margin-bottom: 30px;
  color: #1d3557;
}
.environments-gallery {
  display: flex;
  overflow-x: auto;
  gap: 20px;
  padding: 10px;
  scroll-snap-type: x mandatory;
}
.environment-card {
  flex: 0 0 auto;
  width: 280px;
  height: 400px;
  background-size: cover;
  background-position: center;
  border-radius: 20px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.2);
  position: relative;
  scroll-snap-align: start;
}
.environment-text {
  position: absolute;
  bottom: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.5);
  color: #fff;
  padding: 15px;
  border-radius: 0 0 20px 20px;
}
.environment-text h3 {
  font-size: 1.5rem;
  margin-bottom: 8px;
}
.environment-text p {
  font-size: 1rem;
}
</style>
<!-- Language & Calligraphy Section -->
<div class="calligraphy-section">
  <h2>Art of Calligraphy</h2>
  <p>Drag and drop Arabic words to create your own masterpiece!</p>

  <!-- Calligraphy Elements -->
  <div class="calligraphy-words">
    <div class="word" draggable="true" ondragstart="drag(event)">السلام</div>
    <div class="word" draggable="true" ondragstart="drag(event)">الإمارات</div>
    <div class="word" draggable="true" ondragstart="drag(event)">تراث</div>
    <div class="word" draggable="true" ondragstart="drag(event)">أمل</div>
  </div>

  <!-- Canvas Drop Area -->
  <div id="drop-area" ondrop="drop(event)" ondragover="allowDrop(event)">
    <p>🖌️ Drop words here!</p>
  </div>
</div>

<!-- Add this script inside <script> tag -->
<script>
function allowDrop(ev) {
  ev.preventDefault();
}

function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.innerHTML);
}

function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  var newWord = document.createElement("div");
  newWord.innerHTML = data;
  newWord.className = "dropped-word";
  newWord.style.top = (ev.clientY - 150) + "px";  // adjust position
  newWord.style.left = (ev.clientX - 100) + "px";  // adjust position
  document.getElementById("drop-area").appendChild(newWord);
}
</script>

<!-- Add this style inside <style> tag -->
<style>
/* Calligraphy Section */
.calligraphy-section {
  padding: 60px 20px;
  background: #f7f5f2;
  text-align: center;
}
.calligraphy-section h2 {
  font-size: 2.5rem;
  margin-bottom: 10px;
  color: #6d4c41;
  font-family: 'Amiri', serif; /* Traditional Arabic vibe */
}
.calligraphy-section p {
  font-size: 1.2rem;
  margin-bottom: 30px;
}

.calligraphy-words {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
  margin-bottom: 30px;
}

.word {
  font-family: 'Amiri', serif;
  font-size: 2rem;
  background: #ffd700;
  padding: 10px 20px;
  border-radius: 12px;
  cursor: grab;
  box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
}

#drop-area {
  width: 90%;
  height: 400px;
  margin: auto;
  background: url('https://i.pinimg.com/originals/35/df/d7/35dfd7600a5bc91f81d7e82f3e1a26fc.jpg');
  background-size: cover;
  background-position: center;
  border: 2px dashed #6d4c41;
  border-radius: 20px;
  position: relative;
  overflow: hidden;
}

.dropped-word {
  position: absolute;
  font-family: 'Amiri', serif;
  font-size: 2rem;
  color: #fff;
  text-shadow: 2px 2px 5px #000;
  animation: pop 0.5s ease;
}

@keyframes pop {
  from { transform: scale(0); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}
</style>
