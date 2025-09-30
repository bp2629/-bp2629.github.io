<style>
  body {
    background-color: #fff;
    margin: 0;
    overflow-x: hidden;
    position: relative;
  }

  /* Banner always locked to top */
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

  .logo {
    top: 320px;
    left: 0;
    z-index: 999;
    position: absolute;
  }

  .gallery {
    position: relative;
    width: 100%;
  }
</style>

<body>
  <!-- Top banner -->
  <a href="https://cabezaskateboards.square.site" class="banner">
    <img src="./clickanywheretoprocde.png" />
  </a>

  <!-- Logo -->
  <a href="https://cabezaskateboards.square.site" class="logo">
    <img src="./delbelpcss.png" style="width:100%;" />
  </a>

  <!-- Gallery -->
  <div class="gallery">
    <!-- images here -->
  </div>

  <script>
    const sizes = ["small", "medium", "large"];
    const gallery = document.querySelector(".gallery");
    const images = gallery.querySelectorAll("a");

    // Measure banner + logo area so we start below it
    const bannerHeight = document.querySelector(".banner").offsetHeight;
    const logo = document.querySelector(".logo img");
    const logoBottom = 320 + logo.offsetHeight; // 320px from CSS + logo height

    const galleryStartY = Math.max(bannerHeight, logoBottom) + 50; 
    // +50px padding

    let topPos = galleryStartY;
    const verticalSpacing = 300;

    images.forEach(a => {
      const randomSize = sizes[Math.floor(Math.random() * sizes.length)];
      a.classList.add(randomSize);

      let imgWidth = 200;
      if (randomSize === "small") imgWidth = 140;
      if (randomSize === "medium") imgWidth = 220;
      if (randomSize === "large") imgWidth = 380;

      const maxX = window.innerWidth - imgWidth - 20;
      const randomX = Math.floor(Math.random() * maxX);

      a.style.position = "absolute";
      a.style.top = topPos + "px";
      a.style.left = randomX + "px";

      topPos += verticalSpacing;
    });

    document.body.style.height = (topPos + 500) + "px";
  </script>
</body>
