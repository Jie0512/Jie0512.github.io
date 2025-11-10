<!DOCTYPE html>
<html lang="zh-TW">
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
        main {
            max-width: 800px;
            margin: 20px auto;
            padding: 25px;
            background-color: #ffffff;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
        }
        h2 {
            text-align: center;
            color: #444;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            display: block;
            margin: 10px 0;
        }

        /* --- 彈跳功能 CSS --- */
        #anime-image {
            cursor: pointer; /* 讓滑鼠變成可點擊的手指 */
        }
        
        .is-bouncing {
            animation: bounce-animation 0.8s;
        }

        @keyframes bounce-animation {
            0%   { transform: translateY(0); }
            30%  { transform: translateY(-25px); } /* 往上彈 */
            50%  { transform: translateY(0); }
            70%  { transform: translateY(-10px); }
            100% { transform: translateY(0); }
        }
    </style>
</head>

<body>
    <h2>Jie's personal page</h2>
    <main>
        <p>Click here to view more <a href="#">about me</a>.</p>
        
        <a href="#"><img id="anime-image" src="https://cdn2.ettoday.net/images/8323/8323998.jpg" alt="最近常看的動漫"></a>
        
        <p>Things i love:</p>
        <ul>
            <li>睡覺</li>
            <li>玩電動</li>
        </ul>
    </main>

    <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>

    <script>
        // 等待 HTML 頁面完全載入
        $(document).ready(function() {
        
            // 選擇 ID 為 'anime-image' 的圖片，並綁定點擊事件
            $('#anime-image').on('click', function() {
                
                var image = $(this); // 取得被點擊的圖片
                
                // 幫圖片加上 'is-bouncing' class 來觸發 CSS 動畫
                image.addClass('is-bouncing');
        
                // 在動畫結束後 (800毫秒)，把 class 移除
                // 這樣才能確保下一次點擊時動畫會重播
                setTimeout(function() {
                    image.removeClass('is-bouncing');
                }, 800); // 這個時間 800ms 必須對應 CSS 中的 0.8s
                
            });
        
        });
    </script>

</body>
</html>
