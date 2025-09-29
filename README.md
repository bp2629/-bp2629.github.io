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
      height: 6000px; /* extended for larger images */
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
    a.img-0839 { top: 700px; left: 120px; }
    a.img-0840 { top: 1300px; left: 50px; }
    a.img-0841 { top: 1900px; left: 200px; }
    a.img-0842 { top: 2500px; left: 90px; }
    a.img-0843 { top: 3100px; left: 180px; }
    a.img-0844 { top: 3700px; left: 50px; }
    a.img-0845 { top: 4300px; left: 250px; }
    a.img-0846 { top: 4900px; left: 100px; }
    a.img-0847 { top: 5500px; left: 200px; }
    a.img-0849 { top: 6100px; left: 60px; }
    a.img-0850 { top: 6700px; left: 180px; }
    a.img-0851 { top: 900px; left: 260px; }
    a.img-0853 { top: 1500px; left: 240px; }
    a.img-0854 { top: 2100px; left: 30px; }
    a.img-0855 { top: 2700px; left: 270px; }
    a.img-0856 { top: 3300px; left: 70px; }
    a.img-0857 { top: 3900px; left: 250px; }
    a.img-0876 { top: 4500px; left: 40px; }
    a.img-0877 { top: 5100px; left: 220px; }

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

    /* General image sizing with variation */
    .gallery img {
      box-shadow: 0px 4px 12px black;
    }
    .img-0838 img { width: 300px; }
    .img-0839 img { width: 350px; }
    .img-0840 img { width: 400px; }
    .img-0841 img { width: 500px; }
    .img-0842 img { width: 320px; }
    .img-0843 img { width: 460px; }
    .img-0844 img { width: 380px; }
    .img-0845 img { width: 420px; }
    .img-0846 img { width: 340px; }
    .img-0847 img { width: 480px; }
    .img-0849 img { width: 360px; }
    .img-0850 img { width: 330px; }
    .img-0851 img { width: 500px; }
    .img-0853 img { width: 310px; }
    .img-0854 img { width: 390px; }
    .img-0855 img { width: 470px; }
    .img-0856 img { width: 340px; }
    .img-0857 img { width: 410px; }
    .img-0876 img { width: 300px; }
    .img-0877 img { width: 450px; }
  </style>
</head>
<body>
  <!-- Top banner image -->
 <a href="https://cabezaskateboards.square.site" 
   style="position: absolute; top: 0; left: 0; width: 100%; z-index: 2000;">
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
    <img src="./clickanywheretoprocde.png" style="width: 75px;" />
  </a>

  <!-- === Image Core === -->
  <div class="gallery">
    <a href="https://cabezaskateboards.square.site" class="img-0838"><img src="./olesky_alex_assignment_5-372.jpg" /></a>
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
