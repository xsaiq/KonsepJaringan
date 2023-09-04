# KONSEP JARINGAN

## FTP (File Transfer Protocol)
FTP (File Transfer Protocol) adalah protokol yang digunakan untuk mentransfer file antara komputer melalui jaringan. FTP secara umum menggunakan dua port yang berbeda untuk mengirim data: port 20 dan port 21. Port 21 digunakan untuk menginisiasi sesi kontrol, sementara port 20 (atau port dinamis yang dipilih oleh server) digunakan untuk mengirimkan data yang sebenarnya.

Namun, penting untuk diingat bahwa port 20 dan 21 adalah port TCP (Transmission Control Protocol), bukan UDP (User Datagram Protocol). FTP secara tradisional menggunakan TCP karena protokol ini menjamin pengiriman yang andal dan terurut dari paket-paket data. Dengan demikian, setiap paket yang dikirimkan akan dikonfirmasi oleh penerima, dan jika terjadi kehilangan atau pengulangan paket, protokol akan mengatasi masalah tersebut.

Protokol UDP, di sisi lain, adalah protokol tanpa koneksi yang tidak menjamin pengiriman yang andal atau terurut. Karena FTP melibatkan transfer file yang memerlukan integritas data yang tinggi, penggunaan TCP lebih sesuai. Dengan TCP, file yang dikirimkan melalui FTP dapat dipastikan tiba dengan benar dan tidak rusak.

Meskipun begitu, ada beberapa variasi atau mode FTP yang menggunakan protokol lain, seperti FTPS (FTP Secure) yang dapat menggunakan TLS/SSL untuk enkripsi, serta SFTP (Secure File Transfer Protocol) yang sebenarnya berjalan di atas protokol SSH (Secure Shell). Beberapa protokol pengganti ini mungkin dapat menggunakan port UDP dalam beberapa kasus, tetapi implementasinya dapat berbeda-beda dan mungkin tidak umum digunakan seperti FTP dengan TCP.

---