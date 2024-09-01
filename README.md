<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8" />
    <link rel="shortcut icon" type="image/png" href="./birthdayCake.png"/> 
    <title>Happy Birthday</title>
    <link rel="stylesheet" href="./style.css"> 
    <script src="https://unpkg.com/sweetalert/dist/sweetalert.min.js"></script>
    <script>
        function showMessage() {
            // Lấy element audio
            var audio = document.getElementById('player'); 

            // Kiểm tra xem audio đã được phát chưa
            if (audio.paused) {
                // Nếu chưa phát, bắt đầu phát nhạc
                audio.play(); 
            } 

            // Hiển thị lời nhắn
            swal({
                title: "Lời nhắn", 
                text: "Happy birthday to my little nurse. I'm so glad to have you as a friend for all these years <3 Thank you for everythings", 
                button: {
                    text: "❤️️",
                },
            });
        }
    </script>
</head>
<body>
    <div class="container">
        <div class="balloon">
            <div><span>H</span></div>
            <div><span>A</span></div>
            <div><span>P</span></div>
            <div><span>P</span></div>
            <div><span>Y</span></div>
            <div><span>B</span></div>
            <div><span>I</span></div>
            <div><span>R</span></div>
            <div><span>T</span></div>
            <div><span>H</span></div>
            <div><span>D</span></div>
            <div><span>A</span></div>
            <div><span>Y</span></div>
        </div>
        <div class="avatar">
            <img src="./MyAvatar.jpg" alt="" class="avatar__img" onclick="showMessage()" />
            <h1 onclick="showMessage()" class="avatar__title">Pé iu Diễm My</h1>
        </div>
        <audio id="player" loop> 
            <source src="./music.mp3" type="audio/mp3">
        </audio>
    </div>
</body>
</html>
