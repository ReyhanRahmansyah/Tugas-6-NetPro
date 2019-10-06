# Tugas 6 NetPro
# Anggota Kelompok : 
# Meilyand Evriyan Timor (1301161769)
# Reyhan Rahmansyah (1301160805)
# Reno Butar Butar (1301164724)

# Web Server Design
Berikut adalah Diagram Finite State Machine Web Server :
![Diagram Tugas 6](https://user-images.githubusercontent.com/46934972/66268119-53b11a80-e864-11e9-8c1b-320c02321c6b.png)

Berdasarkan dari diagram FSM diatas. Maka cara kerja dari web server yang kami rancang secara umum bekerja sebagai berikut :
- Browser meminta data web page kepada server, maka instruksi permintaan data oleh browser tersebut akan dikemas di dalam TCP yang merupakan protokol transport dan dikirim ke alamat yang dalam hal ini merupakan protokol berikutnya yaitu HTTP dan atau HTTPS.
- Data yang diminta dari browser ke web server disebut dengan HTTP request kemudian akan dicarikan oleh web server di dalam data server. Jika ditemukan, data tersebut akan dikemas oleh web server dalam TCP dan dikirim kembali ke browser untuk ditampilkan.
- Data yang dikirim dari server ke browser disebut dengan HTTP response. Jika data yang diminta oleh browser tersebut tidak ditemukan oleh web server, maka web server akan menolak permintaan tersebut dan browser akan menampilkan notifikasi Page Not Found atau Error 404.

# Web Server Implementation
Contoh implementasi dari web application yang telah kami rancang :
![Tugas 6 Hasil Implementasi](https://user-images.githubusercontent.com/46934972/66268173-ebaf0400-e864-11e9-99bd-8d0f54d8cc2c.png)

Untuk menjalankannya, tinggal buka terminal dan masuk ke directory src/web-server lalu ketikkan go run *.go di terminal dan buka browser dan ketikkan http://localhost:8080/web/login.html pada halaman web. Maka akan muncul login page seperti pada gambar di atas.
