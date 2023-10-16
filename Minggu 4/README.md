# KONSEP JARINGAN
## Connection Termination
### Pengertian
Connection termination adalah proses penghentian koneksi antara dua perangkat jaringan. Proses ini dapat diinisiasi oleh salah satu perangkat atau oleh keduanya. 

Connection termination biasanya dilakukan dengan cara mengirimkan pesan khusus, seperti pesan FIN (Finish) dalam protokol TCP. Pesan FIN akan memberitahukan perangkat lain bahwa perangkat yang mengirimkan pesan FIN tidak akan mengirimkan data lagi. Perangkat penerima pesan FIN akan membalas dengan pesan ACK (Acknowledgment) untuk mengonfirmasi bahwa pesan FIN telah diterima. 

Connection termination terbagi menjadi 2, yakni full closed dan half closed.

1. **Full Closed**, connection yang telah ditutup sepenuhnya. yang mana kedua host tidak lagi dapat berkomunikasi satu sama lain. Connection full closed biasanya terjadi ketika salah satu host atau perangkat jaringan mengirimkan pesan close. Pesan close ini akan diterima oleh host atau perangkat jaringan lain, dan kemudian connection akan ditutup.
2. **Half Closed**, connection yang hanya ditutup dari satu sisi. Hal ini berarti bahwa satu host atau perangkat jaringan dapat berkomunikasi dengan host atau perangkat jaringan lain, tetapi host atau perangkat jaringan lain tidak dapat berkomunikasi dengan host atau perangkat jaringan pertama. Connection half closed biasanya terjadi ketika salah satu host atau perangkat jaringan mengirimkan pesan close, tetapi host atau perangkat jaringan lain belum siap untuk menutup connection.

### Perbedaan
<table>
<tr>
    <th>Karakteristik</th>
    <th>Full Closed</th>
    <th>Half Closed</th>
</tr>
<tr>
<td>Status</td>
<td>Tertutup sepenuhnya</td>
<td>Tertutup sebagian</td>
</tr>
<tr>
    <td>Kemampuan Komunikasi</td>
    <td>Tidak ada</td>
    <td>Satu arah</td>
</tr>
<tr>
    <td>Cara menutup</td>
    <td>Pesan close dari kedua host atau perangkat jaringan</td>
    <td>Pesan close dari satu host atau perangkat jaringan</td>
</tr>
<tr>
    <td>Contoh</td>
    <td>Menghentikan koneksi ke server web</td>
    <td>Menghentikan pengiriman data ke server web, tetapi masih dapat menerima data dari server web</td>
</tr>
</table>

### Connection Termination Yang Digunakan Pada Tugas Sebelumnya
Listing program pada tugas sebelumnya menggunakan fungsi seperti berikut
```
close(server_fd);
```
Maka dapat disimpulkan program tersebut menggunakan connection termination Full Closed.
***
