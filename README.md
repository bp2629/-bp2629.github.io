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
