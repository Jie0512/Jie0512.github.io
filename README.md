# Jie0512.github.io
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jie's Personal Page</title>

    <style>
        /* 這是您提供的 CSS，我幫您放對了地方 */
        .is-bouncing {
            /* 'bounce-animation' 是我們在下面定義的動畫名稱
               持續 0.8 秒
            */
            animation: bounce-animation 0.8s;
        }

        @keyframes bounce-animation {
            0%   { transform: translateY(0); }
            30%  { transform: translateY(-25px); } /* 往上彈 */
            50%  { transform: translateY(0); }     /* 回到原位 */
            70%  { transform: translateY(-10px); } /* 再小彈一下 */
            100% { transform: translateY(0); }     /* 結束 */
        }

        
        #anime-image {
            cursor: pointer;
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
