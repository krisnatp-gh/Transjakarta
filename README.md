# Latar Belakang
***
Transjakarta adalah perusahaan BUMD (Badan Usaha Milik Daerah) khusus yang dibentuk oleh Pemprov DKI Jakarta untuk mengelola transportasi publik Jakarta. Perusahaan ini mengoperasikan Bus Rapid Transit (BRT) pertama di Asia Tenggara dan Selatan, yang didesain berdasarkan sistem TransMilenio di Bogota, Kolombia. Dengan jalur lintasan terpanjang di dunia (208 km), Transjakarta terus menjadi tulang punggung transportasi massal di Jakarta.

### *Stakeholders*
Transjakarta melibatkan berbagai pemangku kepentingan, termasuk:
- Pemerintah Provinsi DKI Jakarta sebagai pemegang saham tertinggi.
- **Masyarakat DKI dan pengguna Transjakarta**.
- Tim operasi bus dan penyedia layanan pendukung.
- Karyawan dan tenaga kerja Transjakarta.

### Rumusan Masalah
Analisis ini akan berfokus pada data transaksi bulan April 2023. Dataset yang tersedia mencakup informasi detail tentang transaksi penumpang, termasuk waktu perjalanan, rute yang digunakan, serta profil demografis pengguna.

Beberapa fokus utama dalam analisis ini adalah adalah sebagai berikut:
  - Demografi Pengguna
  - Layanan yang harus diprioritaskan
  - Pola penggunaan
  - Rekomendasi untuk peningkatan kualitas layanan

### Data untuk Analisis

Dataset yang digunakan untuk analisis ini merupakan data transaksi Transjakarta selama bulan April 2023 dengan rincian sebagai berikut:

- `transID`: ID unik untuk setiap transaksi pelanggan.

- `payCardID`: Identitas utama pelanggan berupa nomor kartu yang digunakan untuk akses masuk dan keluar.

- `payCardBank`: Nama penerbit kartu bank pelanggan.

- `payCardName`: Nama pelanggan yang tercantum di kartu.

- `payCardSex`: Jenis kelamin pelanggan yang tercantum di kartu.

- `payCardBirthDate`: Tahun kelahiran pelanggan yang tercantum di kartu.

- `corridorID`: ID koridor/rute yang digunakan untuk mengelompokkan rute.

- `corridorName`: Nama koridor/rute yang mencakup titik awal dan akhir perjalanan.

- `direction`: Arah perjalanan, dengan nilai `0` untuk keberangkatan (*Go*) dan `1` untuk kepulangan (*Back*).

- `tapInStops`: ID halte tempat pelanggan melakukan *tap in* (masuk).

- `tapInStopsName`: Nama halte tempat pelanggan melakukan *tap in* (masuk).

- `tapInStopsLat`: Latitude lokasi halte *tap in*.

- `tapInStopsLon`: Longitude lokasi halte *tap in*.

- `stopStartSeq`: Urutan halte dalam koridor/rute untuk *tap in*.

- `tapInTime`: Waktu pelanggan melakukan *tap in*, mencakup tanggal dan waktu.

- `tapOutStops`: ID halte tempat pelanggan melakukan *tap out* (keluar).

- `tapOutStopsName`: Nama halte tempat pelanggan melakukan *tap out* (keluar).

- `tapOutStopsLat`: Latitude lokasi halte *tap out*.

- `tapOutStopsLon`: Longitude lokasi halte *tap out*.

- `stopEndSeq`: Urutan halte dalam koridor/rute untuk *tap out*.

- `tapOutTime`: Waktu pelanggan melakukan *tap out*, mencakup tanggal dan waktu.

- `payAmount`: Jumlah yang dibayarkan oleh pelanggan untuk perjalanan. Beberapa perjalanan gratis, sementara yang lain berbayar.

# Kesimpulan
**Insights**:
- Pengguna **dewasa terbanyak** di semua jenis layanan, sedangkan lansia paling sedikit. **Lebih banyak penumpang perempuan dibanding laki-laki**. **Mayoritas** pengguna **pergi 2 kali dalam sehari**.
- Pengguna akhir pekan **41.46%** total pengguna, tetapi **kontribusi penggunaan dan profit saat weekend tidak signifikan**.
- **Pasangan BRT + Feeder memberi kontribusi terbesar** di jumlah perjalanan dan profit.
- Terdapat **lonjakan jumlah perjalanan** ~10 hari **sebelum Hari Raya Idul Fitri**.
- Terdapat **puncak jumlah perjalanan** pada **pagi dan sore**. Kemungkinan terjadi pula **kemacetan berdekatan dengan jam puncak ini**.
- Beberapa **rute** BRT dan Feeder **terpadat** memiliki **halte yang sama dengan rute terkosong**.

**Rekomendasi**:
- Tingkatkan aksesibilitas/kenyamanan penumpang **wanita** dan **lansia**.
- **Tingkatkan keandalan** layanan di **rute-rute pengguna dewasa tertinggi**, seperti daerah perkantoran.
- Tingkatkan **keandalan layanan BRT dan Feeder**.
- **Kurangi jumlah armada bus di rute-rute terkosong saat akhir pekan**.
- Tingkatkan jumlah armada bus **~10 hari sebelum Idul Fitri**. Sesuaikan jumlah armada setelahnya.
- Pertimbangkan realokasi bus yang sesuai dari **rute terpadat ke rute terkosong**.


