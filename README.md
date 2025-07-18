<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>多語天氣預報</title>
  <style>
    html, body {
      margin: 0;
      height: 100%;
      background: #222;
      color: #fff;
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
    }
    header {
      background: #333;
      padding: 10px;
      text-align: center;
    }
    header button {
      margin: 0 10px;
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      background: #81D4FA;
      cursor: pointer;
      transition: background 0.3s;
    }
    header button:hover {
      background: #4FC3F7;
    }
    iframe {
      flex: 1;
      border: none;
      width: 100%;
    }
  </style>
</head>
<body>
  <header>
    <button onclick="switchLang('ja.html')">日本語</button>
    <button onclick="switchLang('zh.html')">繁體中文</button>
    <button onclick="switchLang('en.html')">English</button>
  </header>

  <iframe id="weatherFrame" src="zh.html"></iframe>

  <script>
    function switchLang(page) {
      document.getElementById('weatherFrame').src = page;
    }
  </script>
</body>
</html>
