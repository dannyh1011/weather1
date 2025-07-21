<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>大廳天氣顯示</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100%;
      background: black; /* 可改品牌色 */
      display: flex;
      flex-direction: column;
    }
    .widget-section {
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .widget-ticker {
      height: 80px; /* ticker 高度可調整 */
    }
    .widget-section div {
      width: 100%;
      height: 100%;
    }
  </style>
</head>
<body>
  <!-- 上方：水平型 weather widget -->
  <div class="widget-section">
    <div id="ww_29697f233d44c" v='1.3' loc='id' a='{"t":"horizontal","lang":"en","sl_lpl":1,"ids":["wl9238"],"font":"Arial","sl_ics":"one_a","sl_sot":"celsius","cl_bkg":"image","cl_font":"#FFFFFF","cl_cloud":"#FFFFFF","cl_persp":"#81D4FA","cl_sun":"#FFC107","cl_moon":"#FFC107","cl_thund":"#FF5722"}'>
      <a href="https://weatherwidget.org/" id="ww_29697f233d44c_u" target="_blank">Widget weather</a>
    </div>
  </div>

  <!-- 下方：ticker 跑馬燈 weather widget -->
  <div class="widget-section widget-ticker">
    <div id="ww_4e7bea93b48e1" v='1.3' loc='id' a='{"t":"ticker","lang":"zh-Hant","sl_lpl":1,"ids":["wl9238"],"font":"Arial","sl_ics":"one_a","sl_sot":"celsius","cl_bkg":"image","cl_font":"#FFFFFF","cl_cloud":"#FFFFFF","cl_persp":"#81D4FA","cl_sun":"#FFC107","cl_moon":"#FFC107","cl_thund":"#FF5722"}'>
      <a href="https://weatherwidget.org/" id="ww_4e7bea93b48e1_u" target="_blank">Widget weather</a>
    </div>
  </div>

  <!-- 兩個 widget script -->
  <script async src="https://app3.weatherwidget.org/js/?id=ww_29697f233d44c"></script>
  <script async src="https://app3.weatherwidget.org/js/?id=ww_4e7bea93b48e1"></script>
</body>
</html>
