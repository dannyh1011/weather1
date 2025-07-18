<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Weather Widgets Multi-language</title>
  <style>
    body {
      margin: 0;
      background: #222;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      overflow: hidden;
    }
    .widget-container {
      width: 100%;
      max-width: 1200px;
      display: grid;
      grid-template-columns: 1fr;
      gap: 20px;
    }
    @media(min-width: 768px) {
      .widget-container {
        grid-template-columns: repeat(3, 1fr);
      }
    }
    iframe, div {
      width: 100%;
      height: 400px;
    }
  </style>
</head>
<body>
  <div class="widget-container">
    <!-- Japanese -->
    <div id="ww_jp" v='1.3' loc='id' a='{"t":"responsive","lang":"ja","sl_lpl":1,"ids":["wl9238"],"font":"Arial","sl_ics":"one_a","sl_sot":"celsius","cl_bkg":"image","cl_font":"#FFFFFF","cl_cloud":"#FFFFFF","cl_persp":"#81D4FA","cl_sun":"#FFC107","cl_moon":"#FFC107","cl_thund":"#FF5722","sl_tof":"3","cl_odd":"#0000000a"}'>
      <a href="https://weatherwidget.org/" id="ww_jp_u" target="_blank">Widget weather</a>
    </div>
    
    <!-- Traditional Chinese -->
    <div id="ww_zh" v='1.3' loc='id' a='{"t":"responsive","lang":"zh-Hant","sl_lpl":1,"ids":["wl9238"],"font":"Arial","sl_ics":"one_a","sl_sot":"celsius","cl_bkg":"image","cl_font":"#FFFFFF","cl_cloud":"#FFFFFF","cl_persp":"#81D4FA","cl_sun":"#FFC107","cl_moon":"#FFC107","cl_thund":"#FF5722","sl_tof":"3","cl_odd":"#0000000a"}'>
      <a href="https://weatherwidget.org/" id="ww_zh_u" target="_blank">Html weather widget</a>
    </div>
    
    <!-- English -->
    <div id="ww_en" v='1.3' loc='id' a='{"t":"responsive","lang":"en","sl_lpl":1,"ids":["wl9238"],"font":"Arial","sl_ics":"one_a","sl_sot":"celsius","cl_bkg":"image","cl_font":"#FFFFFF","cl_cloud":"#FFFFFF","cl_persp":"#81D4FA","cl_sun":"#FFC107","cl_moon":"#FFC107","cl_thund":"#FF5722","sl_tof":"3","cl_odd":"#0000000a"}'>
      <a href="https://weatherwidget.org/" id="ww_en_u" target="_blank">Html weather widget</a>
    </div>
  </div>

  <!-- Scripts -->
  <script async src="https://app3.weatherwidget.org/js/?id=ww_jp"></script>
  <script async src="https://app3.weatherwidget.org/js/?id=ww_zh"></script>
  <script async src="https://app3.weatherwidget.org/js/?id=ww_en"></script>
</body>
</html>
