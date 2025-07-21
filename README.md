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
  </style>
</head>
<body>

  <img class="slide" src="Garden.jpg" alt="">
  <img class="slide" src="SolHotel_M_02.jpg" alt="">

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
    setInterval(nextSlide, 10000); // 每10秒切換
  </script>

</body>
</html>
    showSlides();
  </script>

</body>
</html>
