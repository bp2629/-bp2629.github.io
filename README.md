<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      background-color: rgb(255, 255, 255);
      position: relative;
      height: 5000px; /* increased to allow more spacing */
      overflow-x: hidden;
      margin: 0;
    }
    img {
      display: block;
    }
    a {
      position: absolute;
    }

    /* === Image Core: Mobile default === */
    a.img-0838 { top: 200px; left: 31px; }
    a.img-0839 { top: 600px; left: 120px; }
    a.img-0840 { top: 1000px; left: 50px; }
    a.img-0841 { top: 1400px; left: 200px; }
    a.img-0842 { top: 1800px; left: 90px; }
    a.img-0843 { top: 2200px; left: 180px; }
    a.img-0844 { top: 2600px; left: 50px; }
    a.img-0845 { top: 3000px; left: 250px; }
    a.img-0846 { top: 3400px; left: 100px; }
    a.img-0847 { top: 3800px; left: 200px; }
    a.img-0849 { top: 4200px; left: 60px; }
    a.img-0850 { top: 4600px; left: 180px; }
    a.img-0851 { top: 500px; left: 260px; }
    a.img-0853 { top: 900px; left: 240px; }
    a.img-0854 { top: 1300px; left: 30px; }
    a.img-0855 { top: 1700px; left: 270px; }
    a.img-0856 { top: 2100px; left: 70px; }
    a.img-0857 { top: 2500px; left: 250px; }
    a.img-0876 { top: 2900px; left: 40px; }
    a.img-0877 { top: 3300px; left: 220px; }

    /* === Desktop override === */
    @media (min-width: 768px) {
      a.img-0838 { left: 5%; }
      a.img-0839 { left: 20%; }
      a.img-0840 { left: 35%; }
      a.img-0841 { left: 50%; }
      a.img-0842 { left: 65%; }
      a.img-0843 { left: 80%; }
      a.img-0844 { left: 10%; }
      a.img-0845 { left: 25%; }
      a.img-0846 { left: 40%; }
      a.img-0847 { left: 55%; }
      a.img-0849 { left: 70%; }
      a.img-0850 { left: 85%; }
      a.img-0851 { left: 15%; }
      a.img-0853 { left: 30%; }
      a.img-0854 { left: 45%; }
      a.img-0855 { left: 60%; }
      a.img-0856 { left: 75%; }
      a.img-0857 { left: 90%; }
      a.img-0876 { left: 0%; }
      a.img-0877 { left: 50%; }
    }

    /* General image sizing */
    .gallery img {
      width: 250px; /* base size */
      max-width: 350px;
      box-shadow: 0px 4px 12px black;
    }
  </style>
</head>
<body>
  <!-- Top banner image -->
  <a href="https://cabezaskateboards.square.site" style="top: 0; left: 0; z-index: 1000; position: relative; display: block;">
    <img src="./clickanywheretoprocde.png" style="width: 100%; max-height: 300px; object-fit: cover;" />
  </a>

  <!-- Logo link -->
  <a href="https://cabezaskateboards.square.site" style="top: 320px; left: 0; z-index: 999;">
    <img src="./delbelpcss.png" style="width:100%;" />
  </a>

  <!-- Instagram link text -->
  <a href="https://www.instagram.com/cab3.za/" style="top: 350px; right: 30px; z-index: 999;">Click Here!</a>

  <!-- Instagram icon -->
  <a href="https://www.instagram.com/cab3.za/" style="top: 375px; right: 30px; z-index: 999;">
    <img src="./zoolander0.1488068903.jpg.webp" style="width: 75px;" />
  </a>

  <!-- === Image Core === -->
  <div class="gallery">
    <a href="https://cabezaskateboards.square.site" class="img-0838"><img src="./olesky_alex_assignment_5-369.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0839"><img src="./olesky_alex_assignment_5-373.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0840"><img src="./olesky_alex_assignment_5-374.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0841"><img src="./olesky_alex_assignment_5-376-2.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0842"><img src="./olesky_alex_assignment_5-376.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0843"><img src="./olesky_alex_assignment_5-405.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0844"><img src="./olesky_alex_assignment_5-407.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0845"><img src="./olesky_alex_assignment_5-646.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0846"><img src="./olesky_alex_assignment_5-647.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0847"><img src="./olesky_alex_assignment_5-648.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0849"><img src="./olesky_alex_assignment_5-649.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0850"><img src="./olesky_alex_assignment_5-650.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0851"><img src="./olesky_alex_assignment_5-651.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0853"><img src="./olesky_alex_assignment_5-652.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0854"><img src="./olesky_alex_assignment_5-653.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0855"><img src="./olesky_alex_assignment_5-654.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0856"><img src="./olesky_alex_assignment_5-655.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0857"><img src="./olesky_alex_assignment_5-656.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0876"><img src="./olesky_alex_assignment_5-657.jpg" /></a>
    <a href="https://cabezaskateboards.square.site" class="img-0877"><img src="./olesky_alex_assignment_5-658.jpg" /></a>
  </div>
</body>
</html>
