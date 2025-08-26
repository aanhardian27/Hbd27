<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Ulang Tahun, [Nama Seseorang]!</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="card">
        <div class="card-inner">
            <div class="card-front">
                <h2>Klik untuk membuka</h2>
            </div>
            <div class="card-back">
                <h1>Selamat Ulang Tahun, [Nurfauzy Abdillah]!</h1>
                <img src="https://via.placeholder.com/300x200.png?text=Foto+Kenangan" alt="Foto kenangan" class="birthday-image">
                <p>Halo [Nurfauzy Abdillah],</p>
                <p>Di hari yang spesial ini, aku ingin mengucapkan selamat ulang tahun. Semoga di usiamu yang baru ini, kamu selalu diberikan kebahagiaan, kesehatan, dan semua impianmu bisa tercapai. Ingat, kamu adalah salah satu orang terhebat yang aku kenal.</p>
                <p>Terima kasih sudah menjadi bagian dari hidupku. Aku sangat beruntung memilikimu sebagai teman!</p>
                <p class="signature">- [...]</p>
            </div>
        </div>
    </div>

    <audio id="birthdaySong" loop>
        <source src="https://www.bensound.com/bensound-music/bensound-ukulele.mp3" type="audio/mpeg">
    </audio>

    <script>
        document.querySelector('.card').addEventListener('click', function() {
            this.classList.toggle('is-flipped');
            const song = document.getElementById('birthdaySong');
            if (this.classList.contains('is-flipped')) {
                song.play();
            } else {
                song.pause();
                song.currentTime = 0;
            }
        });
    </script>

</body>
</html>
