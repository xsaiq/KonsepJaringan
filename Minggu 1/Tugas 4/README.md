# KONSEP JARINGAN

## FTP (File Transfer Protocol)

    Kenapa 1 Port FTP Bisa Pakai UDP / TCP?

Port FTP (File Transfer Protocol) sebenarnya menggunakan protokol TCP (Transmission Control Protocol) untuk komunikasi. UDP (User Datagram Protocol) adalah protokol yang berbeda yang memiliki karakteristik yang berbeda. Sebagian besar aplikasi FTP menggunakan TCP karena TCP menawarkan koneksi yang handal dan terjamin, yang sangat penting untuk mentransfer file dengan keamanan dan keakuratan yang tinggi.

FTP menggunakan dua koneksi, yang dikenal sebagai koneksi kontrol (control connection) dan koneksi data (data connection). Koneksi kontrol digunakan untuk mengirim perintah dan menerima tanggapan dari server FTP, sementara koneksi data digunakan untuk mengirim data (misalnya, file yang diunduh atau diunggah).

Protokol FTP dirancang khusus untuk menggunakan TCP sebagai protokol transportasinya. TCP memastikan bahwa data yang dikirimkan antara klien dan server FTP sampai dengan baik, dan jika ada masalah dalam pengiriman, TCP akan mencoba untuk mengirim ulang data tersebut untuk memastikan keakuratan dan keamanan transfer file.

UDP, di sisi lain, adalah protokol yang tidak terjamin, yang berarti data yang dikirimkan menggunakan UDP tidak dijamin akan sampai dengan baik atau dalam urutan yang benar. Karena alasan ini, UDP tidak cocok untuk protokol FTP, yang bergantung pada kehandalan dan keamanan transfer file.

Jadi, meskipun secara teoritis mungkin memungkinkan untuk mencoba menggunakan UDP dengan port yang sama dengan FTP, ini akan menghasilkan transfer file yang tidak handal dan tidak aman, dan ini tidak sesuai dengan desain protokol FTP yang menggunakan TCP untuk kehandalan dan keamanan.

---
