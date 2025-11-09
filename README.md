<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Gallery Layout</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      overflow-x: hidden;
    }

    .banner img {
      width: 100%;
      display: block;
    }

    .logo, .insta-text, .insta-icon {
      position: absolute;
      left: 20px;
      color: white;
    }

    .gallery a img {
      display: block;
      width: 100%;
      border-radius: 10px;
    }

    .gallery a.small { width: 140px; }
    .gallery a.medium { width: 220px; }
    .gallery a.large { width: 270px; }
  </style>
</head>
<body>
  <div class="banner">
    <img src="banner.jpg" alt="Banner">
  </div>

  <div class="logo">Logo</div>
  <div class="insta-text">@username</div>
  <div class="insta-icon">📸</div>

  <div class="gallery">
    <a href="#"><img src="1.jpg"></a>
    <a href="#"><img src="2.jpg"></a>
    <a href="#"><img src="3.jpg"></a>
    <a href="#"><img src="4.jpg"></a>
    <a href="#"><img src="5.jpg"></a>
  </div>

  <script>
    function positionElements() {
      const banner = document.querySelector(".banner img");
      const logo = document.querySelector(".logo");
      const instaText = document.querySelector(".insta-text");
      const instaIcon = document.querySelector(".insta-icon");
      const gallery = document.querySelector(".gallery");
      const images = gallery.querySelectorAll("a");
      const sizes = ["small", "medium", "large"];

      if (!banner.complete || banner.naturalHeight === 0) {
        setTimeout(positionElements, 100);
        return;
      }

      const bannerHeight = banner.offsetHeight;

      logo.style.top = bannerHeight + 10 + "px";
      instaText.style.top = bannerHeight + 40 + "px";
      instaIcon.style.top = bannerHeight + 65 + "px";

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
    }

    // Run once after everything loads
    window.addEventListener("load", positionElements);
  </script>
</body>
</html>
