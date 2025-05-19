![alt text](image.png)
- Program tersebut menjalankan sistem eksekusi asynchronous sederhana menggunakan future kustom bernama `TimerFuture`, yang menunda eksekusi selama dua detik tanpa memblokir thread utama. Saat program dijalankan, ia langsung mencetak “Adie’s Komputer: hey hey”, lalu mengeksekusi task async yang mencetak “howdy!”, kemudian menunggu dua detik secara non-blocking melalui thread terpisah. Setelah waktu habis, task dibangunkan kembali oleh `Waker`, dan mencetak “done!”. Ini menunjukkan bahwa sistem executor, spawner, dan future berjalan dengan benar sesuai mekanisme asynchronous yang diharapkan.


