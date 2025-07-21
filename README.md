<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      width: 100%;
      background: black;
      overflow: hidden;
    }
    .slide {
      position: absolute;
      top: 0; left: 0;
      width: 100vw;
      height: 100vh;
      object-fit: cover;
      display: none;
    }
 <style>
  html, body {
    margin: 0;
    padding: 0;
    height: 100%;
    width: 100%;
    background: black;
    overflow: hidden;
  }
  .slide {
    position: absolute;
    top: 0; left: 0;
    width: 100%;
    height: 100%;
    background-size: cover;
    background-position: center;
    display: none;
  }
</style>
</head>
<body>

  <div class="slide" style="background-image: url('Garden.jpg');"></div>
  <div class="slide" style="background-image: url('SolHotel_M_02.jpg');"></div>

  <script>
    const slides = document.querySelectorAll('.slide');
    let current = 0;

    function showSlide(index) {
      slides.forEach(s => s.style.display = 'none');
      slides[index].style.display = 'block';
    }

    function nextSlide() {
      current = (current + 1) % slides.length;
      showSlide(current);
    }

    showSlide(current);
    setInterval(nextSlide, 10000);
  </script>
