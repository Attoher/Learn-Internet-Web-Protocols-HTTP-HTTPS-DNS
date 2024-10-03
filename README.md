# Internet & Web Protocols (HTTP/HTTPS, DNS)

## 1. **HTTP (Hypertext Transfer Protocol)**

### Overview:
HTTP adalah protokol komunikasi yang digunakan untuk mengirim dan menerima data antar client (browser) dan server di World Wide Web. HTTP bekerja dalam model **client-server**, di mana browser bertindak sebagai client yang membuat permintaan (**request**) dan server mengirimkan respons (**response**).

### Karakteristik HTTP:
- **Stateless**: Setiap request HTTP berdiri sendiri, tidak ada hubungan antara satu request dengan request lainnya.
- **Methods**: HTTP memiliki berbagai metode seperti:
  - **GET**: Mengambil data dari server.
  - **POST**: Mengirim data ke server.
  - **PUT**: Memperbarui data di server.
  - **DELETE**: Menghapus data di server.
- **Status Codes**: Server merespons dengan kode status untuk menunjukkan hasil dari request, contoh:
  - **200 OK**: Request berhasil.
  - **404 Not Found**: Sumber tidak ditemukan.
  - **500 Internal Server Error**: Ada kesalahan di server.

### HTTP Workflow:
1. Client mengirimkan HTTP request (misalnya meminta halaman web).
2. Server menerima request, memprosesnya, dan mengirimkan HTTP response (misalnya mengirim halaman web).

## 2. **HTTPS (Hypertext Transfer Protocol Secure)**

### Overview:
HTTPS adalah versi aman dari HTTP yang menggunakan enkripsi SSL/TLS untuk melindungi data yang dikirim antara client dan server. Ini penting untuk menjaga privasi dan integritas data, terutama pada situs web yang memerlukan informasi sensitif seperti kata sandi atau informasi kartu kredit.

### Keuntungan HTTPS:
- **Keamanan Data**: Semua data yang dikirim melalui HTTPS dienkripsi, sehingga hanya pihak yang berkepentingan yang dapat membaca data tersebut.
- **Integritas Data**: HTTPS mencegah data diubah saat ditransmisikan.
- **Otentikasi**: Sertifikat SSL/TLS digunakan untuk memastikan bahwa server yang terhubung adalah server yang sah.

### HTTPS Workflow:
1. Client terhubung ke server melalui HTTPS.
2. Proses handshake SSL/TLS dilakukan untuk memulai sesi yang aman.
3. Data yang dikirim antara client dan server dienkripsi dan dideskripsikan secara aman.

## 3. **DNS (Domain Name System)**

### Overview:
DNS adalah sistem yang menerjemahkan nama domain yang mudah diingat (seperti `google.com`) menjadi alamat IP numerik (seperti `8.8.8.8`) yang digunakan oleh komputer untuk saling berkomunikasi di jaringan.

### Komponen DNS:
- **Domain**: Nama unik yang digunakan untuk mengidentifikasi situs web.
- **Nameservers**: Server yang bertanggung jawab untuk menjawab query DNS dan memberikan alamat IP yang sesuai dengan nama domain.
- **Zone File**: Berisi catatan DNS untuk domain tertentu, termasuk alamat IP yang terkait dengan subdomain dan layanan lain.

### Tipe Record DNS:
- **A Record**: Memetakan nama domain ke alamat IP IPv4.
- **AAAA Record**: Memetakan nama domain ke alamat IP IPv6.
- **CNAME Record**: Alihkan satu domain ke domain lain.
- **MX Record**: Menunjukkan server email yang digunakan oleh domain.

### DNS Workflow:
1. Browser meminta alamat IP untuk domain tertentu.
2. DNS resolver mencari di cache, jika tidak ditemukan, ia menghubungi DNS server.
3. DNS server memberikan respons dengan alamat IP untuk domain tersebut.
4. Browser menggunakan alamat IP tersebut untuk terhubung ke server dan mengambil data (misalnya halaman web).
