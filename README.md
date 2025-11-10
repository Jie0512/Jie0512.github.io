# Jie0512.github.io
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jie's Personal Page</title>
    
    <style>
        /* --- 基本頁面樣式 --- */
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f4;
            color: #333;
            padding: 20px;
        }

        /* 將主要內容置中，並加上一個最大寬度 */
        main {
            max-width: 800px;
            margin: 20px auto; /* 上下 20px，左右 auto (自動置中) */
            padding: 25px;
            background-color: #ffffff;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
        }

        h2 {
            text-align: center;
            color: #444;
        }

        /* 讓圖片有響應式效果，並加上圓角 */
        img {
            max-width: 100%; /* 圖片寬度不超過容器 */
            height: auto;
            border-radius: 8px;
            display: block; /* 移除圖片底下的空白 */
            margin: 10px 0;
        }

        /* --- 彈跳功能 (CSS + jQuery) --- */

        /* 1. 讓圖片在滑鼠移上去時，顯示「可點擊」的游標 */
        #anime-image {
            cursor: pointer;
            transition: transform 0.2s ease; /* 增加一點平滑過渡 */
        }

        /* 2. 當圖片被點擊時，jQuery 會幫它加上這個 class */
        .is-bouncing {
            /* 'bounce-animation' 是我們在下面定義的動畫名稱
              持續 0.8 秒
            */
            animation: bounce-animation 0.8s;
        }

        /* 3. 定義 "bounce-animation" 這個動畫的內容 */
        @keyframes bounce-animation {
            0%   { transform: translateY(0); }
            30%  { transform: translateY(-25px); } /* 往上彈 */
            50%  { transform: translateY(0); }     /* 回到原位 */
            70%  { transform: translateY(-10px); } /* 再小彈一下 */
            100% { transform: translateY(0); }     /* 結束 */
        }
    </style>
</head>
<h2>Jie's personal page</h2>

<main>

  <p>Click here to view more <a href="#">about me</a>.</p>



  <a href="#"><img src="https://cdn2.ettoday.net/images/8323/8323998.jpg" alt="最近常看的動漫"></a>



  <p>Things i love:</p>

  <ul>

    <li>睡覺</li>

    <li>玩電動</li>

    

  </ul>

</main>
