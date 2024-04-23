# Tugas Praktikum { Pertemuan ke 6 } <img src=https://qph.fs.quoracdn.net/main-qimg-648763cc041459725b62108f4fdf5b91 width="110px" >
|**Nama**|**NIM**|**Kelas**|**Matkul**|
|----|---|-----|------|
|Wawan Suwandi|312310457|TI.23.A5|Basis Data|

# Soal Latihan Praktikum
## 1. Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!

**1. Buat sebuah database dengan nama latihan2**
Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`

![1 1](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/7b4d42ec-fc52-4232-b8be-d9e88fcfba9e)


**2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!**
Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (
    nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran)
    );`

`CREATE TABLE biodata (
    nama varchar (100),
    alamat text
    );`

![1 2](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/7aaedf90-d346-4241-9368-fa08c0315e6d)


**3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!**
Contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15);`

![2 1](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/3d3b2ecf-f933-4c68-a791-b6b980bdad33)


**4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!**
Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int FIRST; `

![2 2](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/8cf21207-cc35-47b9-86b2-8d75d4ee9cdd)


**5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!**
Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah `AFTER`

![3 1](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/a07f93d8-9183-4912-b43c-12a41de36035)


**6. Ubah tipe data kolom id menjadi char(11)!**
Untuk mengubah type data yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);`

![3 2](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/651b7c40-9ecc-4722-907b-a74bd875044c)


**7. Ubah nama kolom phone menjadi hp (char 20)!**
Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

`ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);`

![4 1](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/efb34d86-a9c2-42c5-bdf5-65ef8b46e9ef)

**8. Tambahkan kolom email setelah kolom hp**

![4 2](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/103b774f-ef3d-4888-8a31-99625930db2c)

**9. Hapus kolom keterangan dari tabel!**
Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] DROP nama_field;`

![5 1](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/c04cd53b-b50a-487b-b9ac-4049f0b482d6)

**10. Ganti nama tabel menjadi data_mahasiswa!**
Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];`

[5 2](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/892c17c7-3bc9-4db0-8cc2-eb064b2f834a)

**11. Ganti nama field id menjadi nim!**

![6 1](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/626732a6-923c-4d50-94e8-41d257ffdd5d)

**12. Jadikan nim sebagai PRIMARY KEY!**

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :

tipe index :

- PRIMARY KEY
- UNIQUE KEY
- FULLTEXT

`ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);`

![6 2](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/6597a6f6-ec56-441a-85c6-14325aabbfeb)

**13. Jadikan kolom email sebagai UNIQUE KEY!**

Perintah nya sama seperti diatas, hanya saja diganti menjadi `UNIQUE KEY`

![7](https://github.com/Ws529/Basis-data-Pertemuan6/assets/147570983/f965cfa0-ac94-48a6-ac65-96b30fdea79d)


## 2. Apa Maksud Dari INT(11) ?

- INT(11) Adalah Nama Tipe Datanya Yaitu `Integer` dan Memiliki Panjang 11 Karakter.

## 3. Ketika Kita Melihat Struktur Tabel Dengan Perintah DESC , Ada Kolom Null yang Berisi Yes dan No. Apa Maksudnya ?

- Yaitu Untuk Menjelaskan Bahwa Pada Record yg `NO` Harus diisi , Sedangkan `YES` Boleh Tidak diisi.


### Sekian Tugas Praktikum Saya di Pertemuan kali ini, Jika Masih Ada Yang Salah Saya Mohon Maaf.
### Wassalamualaikum wr.wb. 
