# PA_PBO_KELOMPOK 14
## NAMA KELOMPOK :
### 1. Anggraini Sagita Santia Putri (2209116043)
### 2. Muhammad Nabil		     (2209116046)
## PENGELOLAAN DATA APOTEK PADA RUMAH SAKIT
### DESKRIPSI STUDI KASUS
  Apotek ini adalah sebuah apotek yang tergabung pada Rumah sakit di pusat kota. Apotek ini menyediakan berbagai obat-obatan. Mereka memiliki sistem pengelolaan data obat yang sangat penting untuk menjaga operasi yang efisien dan menyediakan pelayanan yang baik . Apotek ini memiliki persediaan obat yang cukup dan bervariasi. 
	Obat-obatan ini adalah inti dari apotek tersebut. Mereka dikelompokkan berdasarkan jenis , bentuk, dan ukuran yang berbeda. Obat-obat ini juga disimpan dalam kondisi yang terkontrol dan dikelola dengan ketat untuk meminimalkan risiko kesalahan penggunaan obat. Saat dokter meresepkan obat untuk pasien, apoteker mengambil obat dari stok dan memastikan pasien menerima obat yang tepat sesuai dengan petunjuk. Kemudian pasien menerima resep yang mencakup obat-obat yang diperlukan dan dosis yang sesuai.	
	Lalu apoteker ini yang  bertanggung jawab atas pengelolaan obat-obatan dan pemenuhan resep pasien. Mereka menerima resep dari pasien , dan memeriksa stok obat. Apoteker juga berperan penting dalam menjaga persediaan obat yang cukup dan dalam memberikan saran medis terkait penggunaan obat.
### FLOWCHART
![FLOWCHART](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/7d55be26-652e-4ecf-b141-42f5489732af)
	Proses dimulai dari user diminta untuk memilih masuk sebagai apoteker atau pasien jika user memilih sebagai apoteker maka user diminta untuk melakukan login terlebih dahulu dengan menginputkan email dan password yang telah ditentukan, kemudian jika berhasil akan muncul menu pilihan seperti apoteker yang berisi tentang crud data Apoteker , kemudian ada menu pasien yang dimana apoteker akan menginpputkan data pasien yang memiliki resep di menu tersebut, kemudian ada menu resep dimana apoteker akan menginputkan data resep , lalu  ada menu obat yang dimana apoteker akan mengelola , mengubah, dan mennginputkan obat disitu.
 	Selanjutnya ada menu Pasien yang dimana menu pasien ini tidak perlu untuk login karena Untuk memudahkan pasien mengakses informasi dan layanan. Login merupakan proses yang dapat memakan waktu dan membingungkan, terutama bagi pasien yang tidak terbiasa menggunakan teknologi. Dengan tidak perlu login, pasien dapat dengan cepat mengakses informasi dan layanan yang mereka butuhkan. Selanjutnya akan muncul menu pilihan yaitu resep dan menu obat. Pasien hanya bisa mencari data resepnya dan hanya bisa melihat menu obat yang tersedia diapotek tersebut.
### ERD
#### Logical 
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/0196063c-835a-4dab-9529-f3f87d3aba56)
### Relational 
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/9bd24f58-e496-4f81-9089-6e93e219151c)
### HIRARKI 
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/ef193784-64b1-4c01-b1db-280b95b81344)
	Kelas teratas adalah Obat, yang mewakili semua obat yang tersedia di sistem. Kelas tingkat kedua adalah Cair dan Padat, yang mewakili jenis obat yang berbeda. Kelas tingkat ketiga adalah Resep, yang mewakili resep yang dibuat oleh dokter untuk pasien. Kelas tingkat keempat adalah Pasien, yang mewakili pasien yang menggunakan sistem. Hubungan antara kelas-kelas ditunjukkan oleh panah. Panah yang mengarah dari kelas yang lebih tinggi ke kelas yang lebih rendah menunjukkan bahwa kelas yang lebih rendah adalah bagian dari kelas yang lebih tinggi. Obat adalah kelas induk yang memiliki dua kelas turunan, yaitu Cair dan Padat. Kelas Cair dan Padat mewakili jenis obat yang berbeda. Kelas Resep adalah kelas turunan dari kelas Obat dan Pasien. Kelas Resep mewakili resep yang dibuat oleh dokter untuk pasien. Kelas Pasien adalah kelas induk yang tidak memiliki kelas turunan.
### PENJELASAN CODINGAN
#### -ENTITAS-

#### 1. CLASS DATABASE
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/f4a1a620-54ab-4650-8245-e69548b7bb0e)

Gambar diatas merupakan librari untuk menghubungkann dengan  database
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/1d6d790a-2bae-411f-9d81-d48c8c0ffee2)
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/1815fe9f-24fe-43b7-ad52-53c1549ed4b5)
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/780191fd-77c4-467f-a185-db9559307cd0)
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/af166d37-f0e8-4786-ae96-4591723a3d00)
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/7172094b-74b8-4b31-a892-b39aec82f237)

#### 2. CLASS APOTEKER
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/2773d307-3a45-4078-9ec3-22e89be94948)

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/b45e785a-dfec-4332-8f9a-1b2aecdc086a)

Metode ini bertanggung jawab untuk membuat data apoteker baru ke dalam database.
Proses dimulai dengan membuka koneksi ke database.
Membuat pernyataan SQL INSERT untuk memasukkan data ke dalam tabel "Apoteker".
Mengatur nilai parameter dalam pernyataan yang telah disiapkan dengan menggunakan PreparedStatement.
Eksekusi pernyataan SQL menggunakan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika ada kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error) melalui displayErrors(ex).
Akhirnya, koneksi database ditutup, baik operasi berhasil maupun tidak.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/db76e33c-1584-4b45-b840-33964d17294c)

Metode ini digunakan untuk memperbarui data apoteker yang sudah ada dalam database.
Memulai dengan membuka koneksi ke database.
Membuat pernyataan SQL UPDATE untuk memperbarui data dalam tabel "Apoteker" berdasarkan ID yang diberikan.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika ada kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error) melalui displayErrors(ex).
Terakhir, koneksi database ditutup, baik operasi berhasil maupun tidak.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/21412f9f-7168-4990-8e07-15155559c8b5)

Metode ini bertanggung jawab untuk menghapus data apoteker berdasarkan ID yang diberikan.
Membuka koneksi ke database.
Membuat pernyataan SQL DELETE untuk menghapus data dari tabel "Apoteker" berdasarkan ID.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error) melalui displayErrors(ex).
Terakhir, koneksi database ditutup, baik operasi berhasil maupun tidak.

#### 3. CLASS OBAT
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/1c0a6484-456a-4dc2-9f9d-ce09b2ed295b)

Kelas Obat adalah entitas yang merepresentasikan informasi tentang obat di dalam sistem.
Memiliki beberapa atribut untuk menyimpan informasi, seperti id (ID obat), nama_obat (nama obat), stok (jumlah stok obat), tanggal_kadaluarsa (tanggal kadaluarsa obat), dan apoteker_id_apoteker (ID apoteker yang terkait).
Kelas ini meng-extends kelas Database, yang mungkin berisi fungsionalitas untuk berinteraksi dengan database.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/9d206193-e929-411b-834e-c61497375216)

Bertanggung jawab untuk menambahkan data obat baru ke dalam database.
Membuka koneksi ke database.
Menyiapkan pernyataan SQL INSERT untuk memasukkan data ke dalam tabel "obat".
Melakukan konversi dari format tanggal (dalam string) ke java.sql.Date untuk kolom tanggal_kadaluarsa.
Mengatur nilai parameter dalam pernyataan yang disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL menggunakan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error).

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/c63e4204-1539-4199-a15e-0cab9c175c31)

Melakukan pencarian data obat berdasarkan kolom (columnName) dan nilai (value) yang diberikan.
Membuka koneksi ke database.
Membuat pernyataan SQL SELECT untuk mencari data obat berdasarkan kolom yang ditentukan.
Mengatur nilai parameter dalam pernyataan yang disiapkan menggunakan PreparedStatement.
Mengeksekusi pernyataan SQL dengan executeQuery().
Jika data ditemukan, mengisi nilai atribut obat dengan nilai dari database dan mengembalikan keberhasilan operasi dalam bentuk boolean.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/9d53dfcd-33b9-42cf-ac18-14bed944b058)

Bertanggung jawab untuk memperbarui data obat yang sudah ada dalam database.
Membuka koneksi ke database.
Menyiapkan pernyataan SQL UPDATE untuk memperbarui data dalam tabel "obat" berdasarkan ID obat.
Mengatur nilai parameter dalam pernyataan yang disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL menggunakan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error).

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/33ac09d8-02d0-4ef1-a5a2-4034b6ba9bcf)

Bertanggung jawab untuk menghapus data obat dari database berdasarkan ID obat yang diberikan.
Membuka koneksi ke database.
Menyiapkan pernyataan SQL DELETE untuk menghapus data dari tabel "obat" berdasarkan ID obat.
Mengatur nilai parameter dalam pernyataan yang disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL menggunakan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error).

#### 4. CLASS CAIR
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/9edb5b5c-2b72-4dfb-af05-7c61bbbb8a4a)

Kelas Cair merupakan entitas yang merepresentasikan jenis obat cair. Kelas ini memiliki satu atribut yaitu mL, yang menyimpan informasi mili liter dari obat cair. Kelas Cair mewarisi atribut dari kelas Obat

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/b2b00f99-ef12-4401-a0b9-4e1253d54847)

Metode create() di-override dari kelas Obat. Metode ini bertanggung jawab untuk menambahkan data obat cair ke dalam database.
Memulai dengan membuka koneksi ke database.
Membuat pernyataan SQL INSERT untuk memasukkan data ke dalam tabel "cair".
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error) melalui displayErrors(ex).

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/69057c69-7be7-4d27-9cab-9fd2185ad8d9)

Metode update() di-override dari kelas Obat. Metode ini bertanggung jawab untuk memperbarui data obat cair yang sudah ada dalam database.
Mulai dengan membuka koneksi ke database.
Membuat pernyataan SQL UPDATE untuk memperbarui data dalam tabel "cair" berdasarkan ID obat.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error) melalui displayErrors(ex).

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/56a7b7d9-5dd0-4455-85a2-e3270c091250)
Metode delete() di-override dari kelas Obat. Metode ini bertanggung jawab untuk menghapus data obat cair dari database berdasarkan ID obat.
Membuka koneksi ke database.
Membuat pernyataan SQL DELETE untuk menghapus data dari tabel "cair" berdasarkan ID obat.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error) melalui displayErrors(ex).

#### 5. CLASS PADAT

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/cddc80ac-794c-4288-89c5-8c33810ed10d)

Kelas Padat adalah sebuah entitas yang merepresentasikan jenis obat dengan sifat padat.
Kelas ini memiliki satu atribut tambahan yaitu bentuk, yang menyimpan informasi mengenai bentuk fisik dari obat jenis padat.
Kelas Padat mewarisi atribut yang ada pada kelas Obat.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/2ae7fe1c-6f18-41af-b07b-59a04a9f3fb8)

Metode create() di-override dari kelas Obat. Fungsinya adalah untuk menambahkan data obat jenis padat ke dalam database.
Membuka koneksi ke database.
Membuat pernyataan SQL INSERT untuk memasukkan data ke dalam tabel "padat".
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error).

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/08d30aab-cac9-4cda-97fb-e8b52aad4d33)

Metode update() di-override dari kelas Obat. Fungsinya adalah untuk memperbarui data obat jenis padat yang sudah ada dalam database.
Membuka koneksi ke database.
Membuat pernyataan SQL UPDATE untuk memperbarui data dalam tabel "padat" berdasarkan ID obat.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error).

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/2ad40e6a-d1a5-49e2-902d-e6b4668f6a88)

Metode delete() di-override dari kelas Obat. Fungsinya adalah untuk menghapus data obat jenis padat dari database berdasarkan ID obat yang diberikan.
Membuka koneksi ke database.
Membuat pernyataan SQL DELETE untuk menghapus data dari tabel "padat" berdasarkan ID obat.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error).

#### 6. CLASS PASIEN
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/733dbbf2-9e7c-48d0-8a15-dfdd5c62d565)

Kelas Pasien adalah entitas yang berperan dalam merepresentasikan data pasien dalam sistem.
Memiliki beberapa atribut seperti id_pasien (ID pasien), nama_pasien (nama pasien), alamat (alamat pasien), nomorTelepon (nomor telepon pasien), dan email (email pasien).
Kelas Pasien meng-extends kelas Database, yang kemungkinan berisi fungsionalitas untuk berinteraksi dengan database.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/24788eb5-dda6-4ca2-9a30-92ca0fa0d08b)

Metode create() bertanggung jawab untuk menambahkan data pasien baru ke dalam database.
Membuka koneksi ke database.
Membuat pernyataan SQL INSERT untuk memasukkan data ke dalam tabel "pasien".
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL menggunakan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error). Koneksi ke database ditutup dalam blok finally.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/158ca6da-797e-4592-8b48-899282260292)

Metode update() bertanggung jawab untuk memperbarui data pasien yang sudah ada dalam database.
Membuka koneksi ke database.
Membuat pernyataan SQL UPDATE untuk memperbarui data dalam tabel "pasien" berdasarkan ID pasien.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error). Koneksi ke database ditutup dalam blok finally.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/bc1d671a-036c-400d-836e-1624092bc02b)

Metode delete() bertanggung jawab untuk menghapus data pasien dari database berdasarkan ID pasien yang diberikan.
Membuka koneksi ke database.
Membuat pernyataan SQL DELETE untuk menghapus data dari tabel "pasien" berdasarkan ID pasien.
Mengatur nilai parameter dalam pernyataan yang telah disiapkan menggunakan PreparedStatement.
Eksekusi pernyataan SQL dengan executeUpdate() dan mengembalikan keberhasilan operasi tersebut dalam bentuk boolean.
Jika terjadi kesalahan saat eksekusi, akan menampilkan pesan kesalahan (error). Koneksi ke database ditutup dalam blok finally.

#### 7. CLASS RESEP
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/06d81fed-65cf-450d-bd84-3ab78b39dc93)

pada line 16 kelas Resep dideklarasikan sebagai kelas akhir yang mewarisi dari kelas Database. kemudian line 17 sampai line 20 dalah deklarasi variabel anggota yang menggambarkan atribut dari objek Resep. 
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/cd134985-45b4-476e-9ea1-ac620673ef8a)

Gambar diatas merupakan Deklarasi metode create() yang akan menciptakan rekaman baru pada tabel resep. Metode ini akan mengembalikan true jika operasi berhasil dan false jika tidak. Metode ini akan menjalankan operasi CRUD ini dengan menggunakan teknik prepared statement.
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/dff5b73b-69c6-46c5-8e75-ba71ed406ebe)

Gambar diatas merupakan Deklarasi metode update() yang akan mengubah rekaman pada tabel resep. Metode ini akan mengembalikan true jika operasi berhasil dan false jika tidak. Metode ini akan menjalankan operasi CRUD ini dengan menggunakan teknik prepared statement.
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/e8d1d256-0011-43d8-99d6-aea3948b2cb7)

Gambar diatas merupakan Deklarasi metode delete() yang akan menghapus rekaman pada tabel resep. Metode ini akan mengembalikan true jika operasi berhasil dan false jika tidak. Metode ini akan menjalankan operasi CRUD ini dengan menggunakan teknik prepared statement.

![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/4aa47507-74a4-48c2-9d09-96d5da569d0d)
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/80dbbfc7-9f0f-49da-a419-8729965e61cf)
![image](https://github.com/asantiap/PA_PBO_KELOMPOK2/assets/121863819/09fc99d7-6916-41f2-a172-5bc1def727c3)


