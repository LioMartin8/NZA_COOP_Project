# Business Discovery

## 1. Fakta yang Diketahui

- Transaksi cash -> saldo lebih sering terjadi.
- Transaksi saldo -> cash juga tersedia.
- Terdapat aplikasi/provider yang dapat digunakan untuk transaksi ke bank/dompet digital.
- Terdapat aturan biaya/admin berdasarkan nominal.
- Rp5.000 - Rp130.000: admin 3K.
- Rp140.000 - Rp900.000: admin 5K.
- Rp1.000.000 ke atas: admin 10K / 30K.
- Pelanggan cenderung memilih nominal hasil yang genap.
- Setiap karyawan menerima saldo sebesar Rp1.000.000 dari bos untuk periode sekitar 1 minggu.
- Semua transaksi harus dicatat.
- Setoran resmi dilakukan sekitar 1 bulan sekali.
- Laporan internal direncanakan dapat dibuat setiap 1 minggu untuk memantau periode saldo.
## Dpulsa — System Context

Dpulsa (D-Pulsa) merupakan aplikasi/platform PPOB dan distributor produk digital
yang digunakan sebagai provider transaksi.

### Fungsi Utama Dpulsa

Dpulsa menyediakan berbagai produk dan layanan digital, antara lain:

- Pulsa
- Paket data
- Transfer/top-up e-wallet
- Pembayaran PLN
- PDAM
- BPJS
- Pembayaran tagihan lainnya
- Voucher/gift card
- Produk digital lainnya

Pengguna memiliki saldo pada akun Dpulsa. Transaksi dilakukan melalui aplikasi
dan saldo digunakan untuk membayar produk/layanan yang dibeli.

### Biaya Dpulsa

Informasi yang diperoleh:

- Pendaftaran akun: Rp0
- Biaya bulanan: Rp0
- Pulsa, paket data, dan e-wallet: tidak dikenakan admin tambahan dari Dpulsa,
  tetapi produk memiliki harga modal tertentu.
- PPOB seperti PLN, PDAM, dan BPJS: terdapat biaya admin yang bergantung pada
  jenis layanan, sekitar Rp1.500–Rp3.500 per transaksi.
- Deposit saldo melalui transfer bank/Virtual Account: Rp0 sesuai jalur yang
  ditentukan Dpulsa.
- Beberapa metode deposit seperti Indomaret, Alfamart, atau e-wallet tertentu
  dapat memiliki biaya pihak ketiga sekitar Rp1.000–Rp2.500.

### Hubungan Dpulsa dengan NZA Coop

Dpulsa bukan sistem yang sedang dibuat oleh NZA Coop.

Dpulsa berperan sebagai provider/platform eksternal yang menyediakan produk dan
menjadi tempat saldo operasional digunakan untuk melakukan transaksi.

NZA Coop berfungsi sebagai sistem internal untuk:

- mencatat transaksi,
- mencatat penggunaan saldo Dpulsa,
- mencatat uang cash,
- mencatat harga/modal produk,
- mencatat harga yang dibayar pelanggan,
- menghitung margin/keuntungan,
- mengelola hutang pelanggan,
- dan menghasilkan laporan.

### Catatan Penting

Harga modal Dpulsa dan harga jual kepada pelanggan harus dipisahkan.

Contoh:

    Harga produk/nominal       = Rp10.000
    Harga modal Dpulsa         = Rp10.300
    Harga yang dibayar customer = Rp12.000

    Margin bisnis = Rp12.000 - Rp10.300
                  = Rp1.700

Contoh tersebut hanya ilustrasi. Besaran harga jual dan margin NZA Coop
masih harus dikonfirmasi sebagai aturan bisnis.

### Hal yang Belum Dipastikan

- Bagaimana tepatnya NZA Coop menentukan harga jual setiap produk.
- Apakah setiap jenis produk mempunyai aturan margin berbeda.
- Bagaimana biaya/admin Dpulsa dicatat dalam pembukuan NZA Coop.
- Bagaimana saldo Dpulsa direkonsiliasi dengan transaksi yang dicatat NZA Coop.
- Apakah NZA Coop nantinya membutuhkan integrasi/API dengan Dpulsa atau cukup
  menggunakan pencatatan manual.

## 2. Hipotesis

- Customer dapat menentukan nominal saldo yang ingin diterima.
- Customer dapat menentukan nominal cash yang ingin dibayarkan.
- Biaya/admin dapat ditambahkan atau dikurangi dari nominal transaksi.
- Mekanisme transaksi dapat berbeda berdasarkan jenis transaksi.

## 3. Pertanyaan untuk Narasumber

- [ ] Bagaimana alur cash -> saldo?
- [ ] Bagaimana alur saldo -> cash?
- [ ] Apa nama dan fungsi aplikasi/provider yang digunakan?
- [ ] Bagaimana admin sebenarnya dibebankan?
- [ ] Bagaimana aturan Rp1 juta+ 10K / 30K?
- [ ] Data apa yang dicatat setiap transaksi?
- [ ] Bagaimana saldo dan cash dihitung?
- [ ] Bagaimana transaksi gagal/salah ditangani?
- [ ] Bagian mana yang paling merepotkan?

## 4. Hasil Wawancara

Belum ada.

## 5. Perubahan / Temuan Baru

Belum ada.

## 6. Catatan Wawancara

### A. Jenis Transaksi

#### Cash -> Saldo
- Alur:
- Nominal yang umum:
- Admin:
- Saldo yang diterima:
- Aplikasi/provider:
- Data yang dicatat:

#### Saldo -> Cash
- Alur:
- Nominal yang umum:
- Admin:
- Cash yang diterima:
- Aplikasi/provider:
- Data yang dicatat:

### B. Cash & Saldo

- Cash masuk:
- Cash keluar:
- Saldo masuk:
- Saldo keluar:
- Cara mengetahui saldo:
- Cara mengetahui cash:

### C. Aturan Harga/Admin

- Rp5.000–Rp130.000:
- Rp140.000–Rp900.000:
- Rp1.000.000+:
- Aturan lainnya:
- Kapan aturan harga berubah:

### D. Pencatatan

- Media pencatatan:
- Data yang dicatat:
- Siapa yang mencatat:
- Kapan dicatat:
- Laporan harian:
- Laporan bulanan:

### E. Masalah

- Kesalahan yang sering terjadi:
- Transaksi sulit dilacak:
- Perhitungan yang merepotkan:
- Masalah saldo:
- Masalah cash:
- Masalah lainnya:

### F. Aplikasi / Provider

- Nama:
- Fungsinya:
- Cara kerja:
- Saldo/deposit:
- Biaya:
- Batas transaksi:
- Hal lain:

### G. Hal yang Belum Dipahami

- 
