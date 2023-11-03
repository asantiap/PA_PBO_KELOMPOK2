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
#### CLASS RESEP
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

#### CLASS DATABASE

