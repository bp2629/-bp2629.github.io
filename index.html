<script>
function positionElements() {
  const banner = document.querySelector(".banner img");
  const logo = document.querySelector(".logo");
  const instaText = document.querySelector(".insta-text");
  const instaIcon = document.querySelector(".insta-icon");
  const gallery = document.querySelector(".gallery");
  const images = gallery.querySelectorAll("a");

  if (!banner.complete || banner.naturalHeight === 0) {
    // If the banner isn't fully loaded yet, try again shortly
    setTimeout(positionElements, 100);
    return;
  }

  const bannerHeight = banner.offsetHeight;

  // Position elements relative to banner height
  logo.style.top = bannerHeight + 10 + "px";
  instaText.style.top = bannerHeight + 40 + "px";
  instaIcon.style.top = bannerHeight + 65 + "px";

  const sizes = ["small", "medium", "large"];
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

// Recalculate positions after everything loads
window.addEventListener("load", positionElements);

// Recalculate again if screen resizes or rotates (mobile fix)
window.addEventListener("resize", () => {
  // Clear previously added inline positions
  document.querySelectorAll(".gallery a").forEach(a => {
    a.removeAttribute("style");
  });
  positionElements();
});
</script>
