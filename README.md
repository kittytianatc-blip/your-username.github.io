<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Brand Name</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Comic+Neue:wght@700&display=swap');

    body {
      font-family: 'Comic Neue', cursive;
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, #FFC0CB, #FFB6C1); /* Pink gradient */
      text-align: center;
      color: #fff;
    }

    header {
      background-color: #FF69B4;
      color: white;
      padding: 25px 0;
      font-size: 2.5em;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }

    nav {
      margin: 20px 0;
    }

    nav a {
      text-decoration: none;
      color: white;
      background-color: #FF1493;
      padding: 10px 20px;
      border-radius: 10px;
      margin: 0 10px;
      transition: 0.2s;
    }

    nav a:hover {
      background-color: #FF69B4;
    }

    main {
      padding: 40px 20px;
    }

    h2 {
      font-size: 2em;
      margin-bottom: 20px;
    }

    /* Slideshow container */
    .slideshow-container {
      max-width: 600px;
      position: relative;
      margin: auto;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }

    .slides {
      display: none;
      width: 100%;
    }

    .slides img {
      width: 100%;
      display: block;
    }

    /* Download button under slideshow */
    .buy-button {
      display: block;
      margin: 15px auto 30px auto;
      background-color: #FFB6C1;
      border: none;
      padding: 10px 25px;
      border-radius: 10px;
      font-size: 1em;
      cursor: pointer;
      transition: 0.2s;
      color: #fff;
    }

    .buy-button:hover {
      background-color: #FF69B4;
    }

    footer {
      background-color: #FFB6C1;
      padding: 20px;
      font-size: 0.9em;
      color: #fff;
      box-shadow: inset 0 1px 3px rgba(0,0,0,0.2);
    }
  </style>
</head>
<body>

  <header>Your Brand Name 🌸</header>

  <nav>
    <a href="#gallery">Wallpapers</a>
    <a href="#contact">Contact</a>
  </nav>

  <main>
    <h2 id="gallery">Our Pink Wallpapers</h2>

    <div class="slideshow-container">
      <!-- Replace src with your wallpaper images -->
      <div class="slides">
        <img src="wallpaper1.jpg" alt="Wallpaper 1">
      </div>
      <div class="slides">
        <img src="wallpaper2.jpg" alt="Wallpaper 2">
      </div>
      <div class="slides">
        <img src="wallpaper3.jpg" alt="Wallpaper 3">
      </div>
      <!-- Add more slides here -->
    </div>

    <button class="buy-button" onclick="alert('Download current wallpaper!')">Download</button>

    <h2 id="contact">Contact</h2>
    <p>Email: yourname@example.com</p>
    <p>Follow us on social media!</p>
  </main>

  <footer>© 2025 Your Brand Name 🌸 All rights reserved</footer>

  <script>
    let slideIndex = 0;
    showSlides();

    function showSlides() {
      let i;
      let slides = document.getElementsByClassName("slides");
      for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }
      slideIndex++;
      if (slideIndex > slides.length) {slideIndex = 1}
      slides[slideIndex-1].style.display = "block";
      setTimeout(showSlides, 3000); // Change image every 3 seconds
    }
  </script>

</body>
</html>
