# KONSEP JARINGAN

## http.cap ~ telnet-cooked.cap ~ dns.cap

1. http.cap, berisi tangkapan paket HTTP (Hypertext Transfer Protocol), yang digunakan untuk mengirimkan permintaan dan respon antara klien (seperti browser web) dan server. Analisis terhadap http.cap mungkin akan mengungkapkan informasi tentang situs web yang diakses, permintaan yang dibuat, respons dari server, dan potensial data sensitif yang terkandung dalam lalu lintas HTTP.
2. telnet-cooked.cap, berisi tangkapan paket Telnet, yang merupakan protokol jaringan yang digunakan untuk mengakses dan mengendalikan perangkat jarak jauh. Telnet sering kali digunakan untuk mengakses server atau perangkat jaringan dengan cara yang tidak aman karena data yang dikirimkan tidak dienkripsi. Analisis telnet.cap mungkin akan memberikan wawasan tentang perintah yang dijalankan oleh pengguna atau sistem melalui protokol Telnet.
3. dns.cap, berisi tangkapan paket DNS (Domain Name System), yang digunakan untuk menerjemahkan nama domain menjadi alamat IP. Analisis dns.cap mungkin akan mengungkapkan informasi tentang nama domain yang dicari, alamat IP yang dikembalikan, dan pola aktivitas jaringan yang berkaitan dengan layanan DNS.

---