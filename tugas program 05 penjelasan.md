Ubah Tugas 04 dengan membuat database bernama pos.db dengan tabel-tabel sbb:

Tabel toko untuk menampung data dari class Toko dengan kolom-kolom sbb:

id bertipe integer sebagai Primary Key (PK)
nama bertipe String
alamat1 bertipe String
alamat2 bertipe String
alamat3 bertipe String
kota bertipe String
telepon bertipe String
Tabel barang untuk menampung data dari class Barang dan subclass-nya (Curah dan Diskrit) dengan kolom-kolom sbb:

id bertipe integer sebagai Primary Key (PK)
sku bertipe String
nama bertipe String
keterangan bertipe String
stok bertipe integer
jenis bertipe integer. Kolom ini yang akan menentukan apakah ini barang curah atau barang diskrit. Nilainya akan 0 jika barang curah dan 1 jika barang diskrit.
id_toko bertipe integer. Note: harus ada toko dengan id ini, jika tidak ada maka semua operasi akan gagal.
Tabel struk untuk menampung data dari class Struk dengan kolom-kolom sbb:

id bertipe integer sebagai Primary Key (PK)
total_bayar bertipe float
Tabel transaksi untuk menampung data dari class Transaksi dan subclass-nya (Beli dan Jual) dengan kolom-kolom sbb:

id bertipe integer sebagai Primary Key (PK)
tanggal bertipe String
id_barang bertipe integer. Note: harus ada barang dengan id ini, jika tidak ada maka semua operasi akan gagal.
jumlah bertipe float
catatan bertipe String
jenis bertipe integer. Kolom ini yang akan menentukan apakah ini transaksi jual atau transaksi beli. Nilainya akan 0 jika transaksi jual dan 1 jika transaksi beli.
id_struk bertipe integer. Note: harus ada struk dengan id ini, jika tidak ada maka semua operasi akan gagal.
Buat package untuk operasi database sbb:

nama package: basisdata
berisikan satu module: basisdata
module ini berisikan fungsi-fungsi:
buatBasisdata untuk membuat basisdatanya
buatTabelToko untuk membuat tabel toko sesuai spesifikasi di atas.
buatTabelBarang untuk membuat tabel barang sesuai spesifikasi di atas.
buatTabelStruk untuk membuat tabel struk sesuai spesifikasi di atas.
buatTabelTransaksi untuk membuat tabel transaksi sesuai spesifikasi di atas.
Untuk class Toko, Barang, Transaksi, dan Struk
tambahkan method sperti pada praktikum untuk proses CRUD di database.

Koreksi:

Pada constructor Beli dan Jual ada tertinggal parameter tanggal sesudah parameter self.
Nama berkasnya harus:

toko.py untuk class Toko
barang.py untuk class Barang
diskrit.py untuk class BarangDiskrit
curah.py untuk class BarangCurah
transaksi.py untuk class Transaksi
beli.py untuk class Beli
jual.py untuk class Jual
struk.py untuk class Struk
Nama directory-nya harus:

penjualan untuk package penjualan
stok untuk package stok
toko untuk package toko
basisdata untuk package basisdata

buat basisdata,impor module yang dibutuhkan dan lakukan operasi CRUD pada basis data
buat module untuk tiap elemen
basisdata siap
