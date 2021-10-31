# TUGAS-JARKOM-MINGGU-5
- DJIKSTRA

![Screenshot (173)](https://user-images.githubusercontent.com/63788366/139594570-6d5c2ed7-7660-466b-8198-75478adb07f7.png)

Algoritme Dijkstra, (sesuai penemunya  Edsger Dijkstra), adalah sebuah algoritma yang dipakai dalam memecahkan permasalahan jarak terpendek (shortest path problem) untuk sebuah graf berarah (directed graph).

  Algoritma ini dioublikasikan pada tahun 1959  jurnal Numerische Mathematik yang berjudul “A Note on Two Problems in Connexion with Graphs” dan dianggap sebagai algoritma   greedy.

  Algoritma Dijkstra bekerja dengan membuat jalur ke satu simpul optimal pada setiap langkah. Jadi pada langkah ke n, setidaknya ada n node yang sudah kita tahu jalur terpendek.   Langkah-langkah algoritma Dijkstra dapat dilakukan dengan  langkah-langkah berikut:

1. Tentukan titik mana yang akan menjadi node awal, lalu beri bobot jarak pada node pertama ke node terdekat satu per satu, Dijkstra akan melakukan pengembangan pencarian dari satu titik ke titik lain dan ke titik selanjutnya tahap demi tahap.
2. Beri nilai bobot (jarak) untuk setiap titik ke titik lainnya, lalu set nilai 0 pada node awal dan nilai tak hingga terhadap node lain (belum terisi) 2.
3. Set semua node yang belum dilalui  dan set node awal sebagai “Node keberangkatan”
4. Dari node keberangkatan, pertimbangkan node tetangga yang belum dilalui dan hitung jaraknya dari titik keberangkatan. Jika jarak ini lebih kecil dari jarak sebelumnya (yang telah terekam sebelumnya) hapus data lama, simpan ulang data jarak dengan jarak yang baru
5. Saat kita selesai mempertimbangkan setiap jarak terhadap node tetangga, tandai node yang telah dilalui sebagai “Node dilewati”. Node yang dilewati tidak akan pernah di cek kembali, jarak yang disimpan adalah jarak terakhir dan yang paling minimal bobotnya.
6. Set “Node belum dilewati” dengan jarak terkecil (dari node keberangkatan) sebagai “Node Keberangkatan” selanjutnya dan ulangi langkah e.

- UDP

Singkatan dari User Datagram Protocol, merupakan aib satu protokol lapisan transpor TCP/IP yang mendukung komunikasi yang tidak andal (unreliable), tanpa koneksi (connectionless) selang host-host dalam jaringan yang menggunakan TCP/IP. Protokol ini dirumuskan dalam RFC 768.

   UDP sering digunakan dalam beberapa tugas berikut:

1. Protokol yang "ringan" (lightweight): Bagi menghemat sumber daya memori dan prosesor, beberapa protokol lapisan aplikasi membutuhkan penggunaan protokol yang ringan yang dapat memainkan fungsi-fungsi spesifik dengan saling berubah pesan. Contoh dari protokol yang ringan merupakan fungsi query nama dalam protokol lapisan aplikasi Domain Name System.
2. Protokol lapisan aplikasi yang mengimplementasikan layanan keandalan: Jika protokol lapisan aplikasi menyediakan layanan transfer data yang andal, maka kebutuhan terhadap keandalan yang dinegosiasikan oleh TCP pun dijadikan tidak berada. Contoh dari protokol seperti ini merupakan Trivial File Transfer Protocol (TFTP) dan Network File System (NFS)
3. Protokol yang tidak membutuhkan keandalan. Contoh protokol ini merupakan protokol Routing Information Protocol (RIP).
4. Transmisi broadcast: Karena UDP merupakan protokol yang tidak perlu membuat koneksi terlebih dahulu dengan sebuah host tertentu, maka transmisi broadcast pun dimungkinkan. Sebuah protokol lapisan aplikasi dapat mengirimkan paket data ke beberapa tujuan dengan menggunakan alamat multicast atau broadcast. Hal ini kontras dengan protokol TCP yang hanya dapat mengirimkan transmisi one-to-one. Contoh: query nama dalam protokol NetBIOS Name Service.
