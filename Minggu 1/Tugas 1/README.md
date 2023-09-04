# KONSEP JARINGAN

## OSI Layer
OSI (Open Systems Interconnection) adalah model yang menggambarkan cara jaringan komputer berkomunikasi. Model ini terdiri dari tujuh lapisan yang mewakili fungsi-fungsi yang berbeda dalam komunikasi jaringan. Setiap lapisan memiliki tugas khusus, dan data melewati setiap lapisan saat berkomunikasi melalui jaringan. Tujuannya adalah memungkinkan perangkat keras dan perangkat lunak dari berbagai vendor untuk berinteraksi secara efektif dalam komunikasi jaringan.

![osi-layer](assets/osi-layer.jpg)

Gambar di atas merupakan 7 lapisan OSI. Berikut adalah penjelasan dari ketujuh lapisan:

### 1. Lapisan Fisik (Physical Layer)
Lapisan ini bertanggung jawab untuk mentransmisikan bit-bit mentah melalui media fisik seperti kabel, serat optik, atau gelombang radio. Fungsi-fungsi di lapisan ini termasuk sinyal, bit rate, topologi jaringan, serta pengiriman dan penerimaan bit-bit tanpa memperhatikan makna atau struktur bit tersebut.

---
### 2. Lapisan Data Link (Data Link Layer)
Lapisan ini mengelola bagaimana bit-bit diubah menjadi rangkaian data yang lebih besar yang disebut frame. Lapisan ini juga mengatur akses ke media bersama dan mengatasi masalah kesalahan pada lapisan fisik. Lapisan ini dibagi menjadi dua sublapisan: lapisan kontrol akses media (Media Access Control/MAC) dan lapisan kontrol kesalahan (Logical Link Control/LLC).

---
### 3. Lapisan Jaringan (Network Layer)
Lapisan ini mengelola rute data melalui jaringan. Ini termasuk tugas-tugas seperti pemilihan jalur terbaik, pengalamatan logis (seperti alamat IP), dan pengalamatan fisik (seperti alamat MAC).

---
### 4. Lapisan Transport (Transport Layer)
Lapisan ini bertanggung jawab atas pengaturan pengiriman data end-to-end antara host-hos. Ini melibatkan pemecahan data menjadi segmen-segmen, pengelolaan aliran data, pengaturan tipe koneksi (koneksi berorientasi atau tidak berorientasi), dan pengaturan mekanisme pemulihan jika data hilang atau rusak.

---
### 5. Lapisan Session (Session Layer)
Lapisan ini mengatur dan memelihara sesi komunikasi antara dua perangkat. Ini melibatkan manajemen dialog, sinkronisasi data, dan pengendalian aliran.

---
### 6. Lapisan Presentasi (Presentation Layer)
Lapisan ini bertanggung jawab atas penyediaan format data yang dapat dimengerti oleh aplikasi penerima. Ini melibatkan enkripsi, kompresi, konversi karakter, dan manajemen format data.

---
### 7. Lapisan Aplikasi (Application Layer)
Lapisan ini adalah lapisan tertinggi dalam model OSI. Ini berhubungan langsung dengan aplikasi pengguna dan menyediakan layanan komunikasi langsung kepada pengguna, seperti pengiriman email, transfer file, dan browsing web.

---
