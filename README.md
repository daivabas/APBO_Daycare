# APBO_Daycare
ERD
![ERD_Daiva](https://github.com/daivabas/APBO_Daycare/assets/145968640/39648d7e-99ea-4bb1-802f-3ca2b49409bf)
Penjelasan ERD 
1. *OrangTua*:
   - Merupakan entitas yang merepresentasikan orang tua atau wali dari anak-anak yang terdaftar di daycare.
   - Memiliki atribut ID_Ortu sebagai Primary Key untuk mengidentifikasi setiap orang tua secara unik.
   - Atribut lainnya termasuk Nama, Alamat, No_Telepon, dan Email.

2. *Anak*:
   - Merupakan entitas yang merepresentasikan anak yang terdaftar di daycare.
   - Memiliki atribut ID_Anak sebagai Primary Key untuk mengidentifikasi setiap anak secara unik.
   - Memiliki Foreign Key (FK) ID_Ortu yang menghubungkan setiap anak dengan orang tua/wali yang terkait.
   - Memiliki Foreign Key (FK) ID_Staf yang menghubungkan setiap anak dengan staf yang bertanggung jawab.

3. *Staff*:
   - Merupakan entitas yang merepresentasikan staf daycare yang bertanggung jawab atas pengelolaan anak-anak.
   - Memiliki atribut ID_Staf sebagai Primary Key untuk mengidentifikasi setiap staf secara unik.
   - Atribut lainnya termasuk Nama, Jabatan, No_Telepon, dan Email.

4. *Jadwal*:
   - Merupakan entitas yang merepresentasikan jadwal kegiatan dalam sistem daycare.
   - Memiliki atribut ID_Jadwal sebagai Primary Key untuk mengidentifikasi setiap jadwal secara unik.
   - Atribut Tanggal digunakan untuk menunjukkan tanggal jadwal kegiatan.

5. *Absensi*:
   - Merupakan entitas yang merepresentasikan catatan kehadiran anak-anak di daycare.
   - Memiliki atribut ID_Absensi sebagai Primary Key untuk mengidentifikasi setiap catatan absensi secara unik.
   - Memiliki Foreign Key (FK) ID_Anak yang menghubungkan setiap catatan absensi dengan anak yang bersangkutan.


CLASS DIAGRAM
![WhatsApp Image 2024-05-28 at 23 26 05](https://github.com/daivabas/APBO_Daycare/assets/145968640/0ffa6a4a-4410-4ac5-9f66-4c5ed66dd3c9)
Penjelasan DiagramClass nya

1. *OrangTua*:
   - Kelas yang merepresentasikan orang tua atau wali dari anak-anak yang terdaftar di daycare.
   - Memiliki atribut seperti ID_Ortu, Nama, Alamat, No_Telepon, dan Email.
   - Memiliki method untuk mengatur dan mengambil informasi tentang orang tua, seperti setNama, getNama, setAlamat, dan getEmail.

2. *Anak*:
   - Kelas yang merepresentasikan anak yang terdaftar di daycare.
   - Memiliki atribut seperti ID_Anak, Nama, Tanggal_Lahir, ID_Ortu, dan ID_Staf.
   - Memiliki method untuk mengatur dan mengambil informasi tentang anak, seperti setNama, getTanggalLahir, setIDOrtu, dan getIDStaf.

3. *Staff*:
   - Kelas yang merepresentasikan staf daycare yang bertanggung jawab atas pengelolaan anak-anak.
   - Memiliki atribut seperti ID_Staf, Nama, Jabatan, No_Telepon, dan Email.
   - Memiliki method untuk mengatur dan mengambil informasi tentang staf, seperti setNama, getJabatan, dan getEmail.

4. *Jadwal*:
   - Kelas yang merepresentasikan jadwal kegiatan dalam sistem daycare.
   - Memiliki atribut seperti ID_Jadwal dan Tanggal.
   - Memiliki method untuk mengatur dan mengambil informasi tentang jadwal, seperti setTanggal dan getDaftarKegiatan.

5. *Absensi*:
   - Kelas yang merepresentasikan catatan kehadiran anak-anak di daycare.
   - Memiliki atribut seperti ID_Absensi, ID_Anak, Tanggal, Waktu_Masuk, dan Waktu_Keluar.
   - Memiliki method untuk mengatur dan mengambil informasi tentang absensi, seperti setTanggal, getWaktuMasuk, dan getWaktuKeluar.

6. *Aktivitas*:
   - Kelas yang merepresentasikan aktivitas yang dilakukan di daycare.
   - Memiliki atribut seperti ID_Aktivitas, Nama, dan Deskripsi.
   - Memiliki method untuk mengatur dan mengambil informasi tentang aktivitas, seperti setNama dan getDeskripsi.

7. *LaporanAktivitas*:
   - Kelas yang merepresentasikan laporan aktivitas harian anak-anak di daycare.
   - Memiliki atribut seperti ID_Laporan, ID_Anak, Tanggal, dan Catatan.
   - Memiliki method untuk mengatur dan mengambil informasi tentang laporan aktivitas, seperti setTanggal dan getCatatan.


USE CASE

<img width="454" alt="USE CASE" src="https://github.com/daivabas/APBO_Daycare/assets/145968640/f9b0f52b-4a90-43cf-ba2a-5dbca1e0a6ec">
