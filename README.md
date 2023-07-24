let's try game snake
https://asep38.github.io/game-snake.github.io/

<img src="https://user-images.githubusercontent.com/112145050/255480482-4206a778-9452-41cf-8663-eebdabaf15fe.png" />

# Deskripsi
Game Snake adalah permainan video klasik yang sederhana namun adiktif, di mana pemain mengendalikan seekor ular untuk mengumpulkan makanan (apel) yang tersebar di area permainan. Setiap kali ular memakan apel, panjangnya akan bertambah. Tujuan utama pemain adalah bertahan selama mungkin dan mencetak skor tertinggi dengan mengendalikan gerakan ular secara bijaksana.

# Cerita
Cerita dimulai pada tahun 1976, ketika seorang insinyur komputer bernama Gremlin Industries menciptakan permainan sederhana berjudul "Blockade." Permainan ini merupakan permainan multi-pemain yang mengharuskan pemain mengendalikan garis bergerak di layar untuk menghindari tabrakan dengan dinding atau garis lawan. Blockade menjadi hit di arcade dan menjadi salah satu permainan video pertama yang menampilkan aspek permainan yang mirip dengan game Snake.

Pada tahun 1977, Atari merilis permainan bernama "Surround," yang merupakan adaptasi dari Blockade. Surround memperkenalkan mode single-player, di mana pemain harus mengendalikan garis yang terus bertambah panjang saat mereka bergerak di layar. Jika garis tersebut menabrak dinding atau dirinya sendiri, permainan berakhir. Meskipun masih sederhana, permainan ini menarik perhatian banyak orang dan menjadi populer di arcade.

Namun, kesuksesan dan popularitas sesungguhnya dari game Snake bermula pada tahun 1997 ketika Nokia, salah satu perusahaan telekomunikasi terkemuka, merilis ponsel bermodel Nokia 6110. Ponsel ini dilengkapi dengan permainan sederhana yang disebut "Snake." Permainan ini menjadi bagian dari paket permainan standar pada banyak ponsel Nokia yang dirilis selama tahun-tahun berikutnya.

# Fungsi Yang saya gunakan
- gameLoop(): Fungsi ini merupakan loop permainan yang memanggil fungsi show() secara berkala dengan interval 50ms (1000ms / 20fps) untuk memperbarui dan menggambar permainan.

- pauseBtn.addEventListener("click", () => {...}): Fungsi ini berfungsi untuk menghentikan permainan dengan menghentikan interval gameLoop ketika tombol "Pause" ditekan.

- playBtn.addEventListener("click", () => {...}): Fungsi ini berfungsi untuk melanjutkan permainan dengan memulai interval gameLoop kembali ketika tombol "Play" ditekan.

- show(): Fungsi ini memanggil fungsi update() dan draw() untuk memperbarui dan menggambar elemen-elemen permainan di layar.

- update(): Fungsi ini melakukan beberapa perhitungan dan pembaruan penting pada permainan, termasuk pergerakan ular, memeriksa tabrakan ular dengan dirinya sendiri, menghitung skor, dan memeriksa apakah ular menyentuh dinding atau apel.

- checkSelfCollision(): Fungsi ini memeriksa apakah kepala ular (headTail) bertabrakan dengan bagian tubuh lainnya dalam bentuk ular sendiri. Jika terjadi tabrakan, permainan akan berakhir dan memanggil fungsi gameOver().

- gameOver(): Fungsi ini berfungsi untuk menghentikan permainan, menampilkan popup game over, dan menampilkan skor akhir ular.

- eatApple(): Fungsi ini memeriksa apakah ular memakan apel. Jika kepala ular berada di posisi apel, maka ular akan bertambah panjang dan apel akan dihapus dan digantikan dengan apel baru.

- checkHitWall(): Fungsi ini memeriksa apakah kepala ular menyentuh dinding (keluar dari batas layar). Jika ular menyentuh dinding, maka posisi ular akan diubah agar ular kembali muncul dari sisi yang berlawanan (seperti klasik game snake).

- draw(): Fungsi ini menggambar elemen-elemen permainan seperti latar belakang, tubuh ular, apel, dan skor pada kanvas.

- createRect(x, y, width, height, color): Fungsi ini digunakan untuk menggambar persegi berwarna pada kanvas.

- window.addEventListener("keydown", (event) => {...}): Fungsi ini menangani event saat tombol panah ditekan. Saat tombol panah ditekan, arah pergerakan ular akan diubah berdasarkan input pemain.
