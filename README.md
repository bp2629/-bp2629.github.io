<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      background-color: #fff;
      margin: 0;
      overflow-x: hidden;
      position: relative;
    }

    /* === Banner === */
    .banner {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 2000;
    }

    .banner img {
      width: 100%;
      max-height: 300px;
      object-fit: cover;
      display: block;
    }

    /* === Logo === */
    .logo {
      position: absolute;
      left: 0;
      z-index: 1500;
    }

    .logo img {
      width: 100%;
      height: auto;
      display: block;
    }

    /* === Instagram === */
    .insta-text {
      position: absolute;
      right: 30px;
      z-index: 1600;
    }

    .insta-icon {
      position: absolute;
      right: 30px;
      z-index: 1600;
    }

    .insta-icon img {
      width: 75px;
      height: auto;
      display: block;
    }

    /* === Gallery === */
    .gallery {
      position: relative;
      width: 100%;
    }

    .gallery a img {
      box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.6);
      display: block;
    }

    .small img {
      width: 140px;
    }

    .medium img {
      width: 220px;
    }

    .large img {
      width: 380px;
    }
  </style>
</head>
<body>
  <!-- Top banner -->
  <a href="https://cabezaskateboards.square.site" class="banner">
    <img src="./clickanywheretoprocde.png" />
  </a>

  <!-- Logo -->
  <a href="https://cabezaskateboards.square.site" class="logo">
    <img src="./delbelpcss.png" />
  </a>

  <!-- Instagram -->
  <a href="https://www.instagram.com/cab3.za/" class="insta-text">Click Here!</a>
  <a href="https://www.instagram.com/cab3.za/" class="insta-icon">
    <img src="./zoolander0.1488068903.jpg.webp" />
  </a>

  <!-- === Gallery === -->
  <div class="gallery">
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-374.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-376-2.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-376.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-405.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-407.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-646.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-647.jpg" /></a>
    <!-- 372 + 373 in the middle -->
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-372.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-373.jpg" /></a>
    <!-- continue -->
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-648.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-649.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-650.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-651.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-652.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-653.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-654.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-655.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-656.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-657.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-658.jpg" /></a>
  </div>

  <script>
  window.onload = function() {
    const sizes = ["small", "medium", "large"];
    const banner = document.querySelector(".banner img");
    const logo = document.querySelector(".logo");
    const instaText = document.querySelector(".insta-text");
    const instaIcon = document.querySelector(".insta-icon");

    // Place logo just under banner
    const bannerHeight = banner.offsetHeight;
    logo.style.top = bannerHeight + 10 + "px"; // small gap
    instaText.style.top = bannerHeight + 40 + "px";
    instaIcon.style.top = bannerHeight + 65 + "px";

    const gallery = document.querySelector(".gallery");
    const images = gallery.querySelectorAll("a");

    // Now gallery starts at the same height as the logo
    const galleryStartY = bannerHeight + 10; 

    let topPos = galleryStartY;
    const verticalSpacing = 320;

    images.forEach(a => {
      const randomSize = sizes[Math.floor(Math.random() * sizes.length)];
      a.classList.add(randomSize);

      let imgWidth = 200;
      if (randomSize === "small") imgWidth = 140;
      if (randomSize === "medium") imgWidth = 220;
      if (randomSize === "large") imgWidth = 270;

      const maxX = window.innerWidth - imgWidth - 20;
      const randomX = Math.floor(Math.random() * maxX);

      a.style.position = "absolute";
      a.style.top = topPos + "px";
      a.style.left = randomX + "px";

      topPos += verticalSpacing;
    });

    document.body.style.height = (topPos + 500) + "px";
  };
  </script>
</body>
</html>
