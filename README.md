<!DOCTYPE html>
<html lang="ja">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <link rel="stylesheet" href="kafe.css">
    <meta name="description" content="CSSファイルをHTMLに読み込む基本的な方法を解説しています。初心者向けにわかりやすく紹介。">
    <style>
        body {
            background-image: url(kafe.img/名称未設定のデザイン\ \(28\).png);
            background-position: center 5%;
            background-size: 100%;
            background-color: rgba(245, 207, 136, 0.815);
        }
    </style>
</head>

<body>
    <div class="container">
        <div style="text-align: center;">
            <div class="yoko">
                <style></style>
                <img src="kafe.img/Sora Cafe (1).png">
                <p>　　</p>
                <a href="#toppu"><button class="button-49">トップ</button></a>
                <p>　　</p>
                <a href="menu.html"><button class="button-49">メニュー</button></a>
                <p>　　　　　　</p>
            </div>
            <div class="hamburger" onclick="toggleMenu()">
                <span></span>
                <span></span>
                <span></span>
            </div>

            <!-- メニュー（右側からスライド） -->
            <nav id="nav-menu">
                <ul>
                    <li><a href=#こだわり>こだわり</a></li>
                    <li><a href="menu.html">メニュー</a></li>
                    <li><a href="#ei">営業時間</a></li>
                    <li><a href="#予約">予約</a></li>
                    <li><a href="#住所">住所</a></li>
                    <li><a href="https://form.run/@kawano--RE2aCKdmh2TV75hCU1kI">お問い合わせ</a></li>
                </ul>
            </nav>

            <script>
                function toggleMenu() {
                    document.getElementById('nav-menu').classList.toggle('active');
                }
            </script>






        </div>

        <div style="align-items: center;">
            <div class="box-010">
                <span>お知らせ</span>
                <p>クリスマスに新商品！！</p>
                <br><br><br>
            </div>
            <div class="slideshow-container">
                <div class="slide">
                    <img src="kafe.img/名称未設定のデザイン (13).png" alt="スライド1">
                </div>
                <div class="slide">
                    <img src="kafe.img/名称未設定のデザイン (14).png" alt="スライド2">
                </div>
                <div class="slide">
                    <img src="kafe.img/名称未設定のデザイン (15).png" alt="スライド3">
                </div>
            </div>

            <script>
                let slideIndex = 0;
                const slides = document.getElementsByClassName("slide");

                function showSlides() {
                    for (let i = 0; i < slides.length; i++) {
                        slides[i].style.display = "none";
                    }
                    slideIndex++;
                    if (slideIndex > slides.length) { slideIndex = 1; }
                    slides[slideIndex - 1].style.display = "block";
                    setTimeout(showSlides, 3000); // 3秒ごとに切り替え
                }

                showSlides();
            </script>
            <br>
            <div style="text-align: center; color: rgb(255, 187, 86);">
                <div class="box-003">
                    <h1>concept</h1>
                    <p style="font-size: x-large;">家族みんなでくつろげる小さなカフェ</p>

                </div>
                <br><br>
                <div class="box-003">
                    <h1 id="こだわり">こだわり</h1>
                    <p style="font-size: x-large;">
                        家族でも安心していただけるように、素材から空間づくりまで、一つひとつに想いをこめています。お子様にも安心して食べていただけるよう。添加物をできるだけ使わず、地元の新鮮な食材を使用。木のぬくもりを感じる店内は、ベビーカーでも入りやすく、ゆったりとくつろげる空間になっています
                    </p>
                </div>
            </div>
        </div>
        <br><br><br><br><br>

        <div class="box-003">
            <div class="yoko">
                <img src="kafe.img/名称未設定のデザイン (19).png" style="width: 30%; height: auto;">
                <img src="kafe.img/名称未設定のデザイン (20).png">
                <p>　</p>
                <img src="kafe.img/名称未設定のデザイン (18).png" style="width: 30%; height: auto;">
            </div>
            <div class="container">
                <div class="yoko">
                    <p>ベビーカー置き場を設置!!</p>
                    <p>　　　　　　　　　店内禁煙</p>
                    <p>　　　　　　　　　　　　かわいい店内で！</p>
                </div>
            </div>
        </div>
    </div>
    </div>
    </div>
    <br><br><br>
    <div class="box-003">
        <h1 id="ei">営業時間</h1>
        <p style="font-size: x-large;">土曜日 09:30-20:00 <br>
            日曜日 09:00-20:00 <br>
            月曜日 09:30-20:00 <br>
            火曜日 09:30-20:00 <br>
            水曜日 09:30-20:00 <br>
            木曜日 09:30-20:00 <br>
            金曜日 09:30-20:00 <br>

            ※祝日の営業時間は、9:00-20:00となります。</p>
    </div>
    <br>
    <div class="box-003">
        <h1 id="住所">住所</h1>
        <p>〒533-0013 大阪府大阪市東淀川区豊里５丁目１４</p>
        <iframe
            src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d11684.283584029312!2d135.5423003978567!3d34.73564863461093!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sja!2sjp!4v1760193608349!5m2!1sja!2sjp"
            width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
    <br>

    <div class="yoko">

        <p>　　　　　　　　　　　　　</p>
        <a href="https://www.instagram.com/kawano11293?igsh=MXgzbjByY2U3Zmk5dA%3D%3D&utm_source=qr"><img
                src="kafe.img/名称未設定のデザイン (25).png" alt=""></a>
        <p>　　　</p>

        <button class="like-button" onclick="addLike()"><img src="kafe.img/名称未設定のデザイン (27).png" alt=""> <span
                id="like-count">0</span></button>

        <script>
            let likeCount = 0;

            function addLike() {
                likeCount++;
                document.getElementById('like-count').innerText = likeCount;
            }
        </script>
        <p>　　　</p>
        <img src="kafe.img/名称未設定のデザイン (26).png" alt="">

    </div>
    </div>

</body>

</html>
