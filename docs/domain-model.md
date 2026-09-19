# NZA Coop — Domain Model V0.1

## Tujuan

Domain model ini menggambarkan objek utama dalam operasional NZA Coop
berdasarkan informasi yang sudah diketahui saat ini.

Model ini masih dapat berubah apabila ditemukan aturan bisnis baru.

---

## Entity

### Employee

Karyawan/agen yang melakukan transaksi.

Data awal:

- id
- name
- active

---

### Customer

Pelanggan yang melakukan transaksi atau memiliki hutang.

Data awal:

- id
- name
- contact
- active

---

### Transaction

Catatan setiap transaksi yang dilakukan oleh employee untuk customer.

Data awal:

- id
- timestamp
- employee
- customer
- transaction_type
- product
- amount
- cost
- customer_paid
- status
- notes

Contoh transaction_type:

- cash_to_balance
- balance_to_cash
- pulsa
- data
- ewallet
- ppob
- other

---

### Dpulsa Balance

Saldo operasional yang diberikan kepada employee dan digunakan
untuk melakukan transaksi melalui Dpulsa.

Data awal:

- employee
- initial_balance
- current_balance

---

### Loan

Catatan uang yang dipinjam oleh customer.

Data awal:

- id
- customer
- amount
- paid_amount
- remaining_amount
- borrowed_at
- status

---

### Reporting Period

Periode yang digunakan untuk melakukan pencatatan dan rekonsiliasi.

Data awal:

- id
- employee
- start_date
- end_date
- initial_balance

Catatan:

- Alokasi saldo dari boss kepada employee diketahui berlangsung sekitar
  satu minggu.
- Setoran resmi kepada boss diketahui dilakukan satu bulan sekali.
- Periode laporan internal masih perlu dikonfirmasi.

---

## Relationship

Employee:

    Employee
       │
       ├── melakukan ──> Transaction
       │
       └── memiliki ──> Dpulsa Balance

Customer:

    Customer
       │
       ├── melakukan ──> Transaction
       │
       └── memiliki ──> Loan

Reporting Period:

    Reporting Period
       │
       ├── mencakup ──> Transaction
       └── mencatat ──> Dpulsa Balance

---

## Catatan Ketidakpastian

Beberapa bagian belum dianggap sebagai aturan final:

- aturan harga jual,
- aturan margin,
- mekanisme biaya/admin,
- detail perubahan saldo setelah setiap transaksi,
- mekanisme cash masuk/keluar,
- hubungan transaksi dengan periode laporan,
- aturan transaksi di atas Rp150.000,
- mekanisme pembayaran hutang.