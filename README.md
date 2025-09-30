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
      overflow-x: hidden; /* 🚫 disables horizontal scroll */
      position: relative;
    }

    img {
      display: block;
      max-width: 100%;
      height: auto;
    }

    a {
      position: absolute;
    }

    /* === Logo + Links === */
    .logo {
      top: 320px;
      left: 0;
      z-index: 999;
    }

    /* === Gallery === */
    .gallery {
      position: relative;
      margin-top: 500px; /* 🚀 pushes gallery down past logo */
      width: 100%;
    }

    .gallery a {
      position: absolute; /* will place at random X + stacked Y */
    }

    .gallery img {
      box-shadow: 0px 4px 12px black;
      height: auto;
    }

    /* === Varied Sizes === */
    .small img { width: 140px; }
    .medium img { width: 220px; }
    .large img { width: 380px; }
  </style>
</head>
<body>
  <!-- Top banner -->
  <a href="https://cabezaskateboards.square.site" 
     style="position:absolute; top:0; left:0; width:100%; z-index:2000;">
    <img src="./clickanywheretoprocde.png" style="width:100%; max-height:300px; object-fit:cover;" />
  </a>

  <!-- Logo -->
  <a href="https://cabezaskateboards.square.site" class="logo">
    <img src="./delbelpcss.png" style="width:100%;" />
  </a>

  <!-- Instagram link text + icon -->
  <a href="https://www.instagram.com/cab3.za/" style="top:350px; right:30px; z-index:999;">Click Here!</a>
  <a href="https://www.instagram.com/cab3.za/" style="top:375px; right:30px; z-index:999;">
    <img src="./zoolander0.1488068903.jpg.webp" style="width:75px;" />
  </a>

  <!-- === Image Core Gallery === -->
  <div class="gallery">
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-372.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-373.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-374.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-376-2.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-376.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-405.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-407.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-646.jpg" /></a>
    <a href="https://cabezaskateboards.square.site"><img src="./olesky_alex_assignment_5-647.jpg" /></a>
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
    // Randomize sizes + X positions
    const sizes = ["small", "medium", "large"];
    const gallery = document.querySelector(".gallery");
    const images = gallery.querySelectorAll("a");

    let topPos = 0; // starting vertical position
    const verticalSpacing = 300; // space between rows

    images.forEach(a => {
      // Random size
      const randomSize = sizes[Math.floor(Math.random() * sizes.length)];
      a.classList.add(randomSize);

      // Measure image width (based on size class)
      let imgWidth = 200;
      if (randomSize === "small") imgWidth = 140;
      if (randomSize === "medium") imgWidth = 220;
      if (randomSize === "large") imgWidth = 380;

      // Random X, ensuring it fits in viewport
      const maxX = window.innerWidth - imgWidth - 20; // padding
      const randomX = Math.floor(Math.random() * maxX);

      // Assign positions
      a.style.top = topPos + "px";
      a.style.left = randomX + "px";

      // Increment vertical stacking
      topPos += verticalSpacing;
    });

    // Extend page height to fit images
    document.body.style.height = (topPos + 500) + "px";
  </script>
</body>
</html>
