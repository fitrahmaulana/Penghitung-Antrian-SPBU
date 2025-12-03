# ⛽ Kalkulator Estimasi Antrian SPBU

Sebuah *web tool* sederhana untuk menghitung estimasi waktu tunggu antrian BBM. Proyek ini dirancang khusus merespons kondisi antrian panjang di Provinsi Aceh, namun dapat diterapkan secara universal di SPBU mana pun.

## 💡 Latar Belakang
Program ini tercipta dari observasi langsung terhadap krisis BBM dan fenomena antrian panjang yang terjadi di Banda Aceh. Banyak masyarakat yang terjebak dalam antrian selama berjam-jam (dari pagi hingga siang) tanpa kepastian estimasi waktu.

## 🎯 Tujuan & Manfaat
Membantu pengguna mengambil keputusan yang lebih cerdas (*Decision Making Support*):
* Mengetahui perkiraan waktu tunggu berdasarkan panjang antrian.
* Mempertimbangkan apakah "Layak" (*worth it*) untuk ikut mengantri atau sebaiknya mencari alternatif SPBU lain.

## ⚙️ Logika & Transparansi Perhitungan
Sistem ini menggunakan parameter rata-rata kondisi lapangan (kondisi antrian rapat):

| Parameter | Nilai | Keterangan |
| :--- | :--- | :--- |
| **Panjang Rata-rata Motor** | 2.1 Meter | Asumsi motor berbaris rapat. |
| **Durasi Pelayanan** | 1.5 Menit | Estimasi dorong motor, buka jok, isi bensin, hingga pembayaran selesai. |

## ⚠️ Disclaimer (Batasan Sistem)
Hasil perhitungan adalah **estimasi teoritis**. Kondisi aktual di lapangan dapat berbeda (bisa lebih cepat atau lambat) tergantung pada variabel eksternal yang tidak terduga, seperti:
* Keterampilan petugas SPBU.
* Kendala teknis (mesin macet/genset rusak).
* Stok BBM habis di tengah antrian.

Namun, dalam kondisi normal, selisih perhitungan ini dirancang agar tidak menyimpang terlalu jauh dari realita.

## ✨ Fitur Baru (2025)

### 🎨 Mode Terang/Gelap
* Toggle tema untuk kenyamanan mata di berbagai kondisi pencahayaan
* Preferensi tema tersimpan otomatis di browser

### 📋 Riwayat Perhitungan
* Menyimpan hingga 10 perhitungan terakhir ke LocalStorage browser
* Akses cepat ke perhitungan sebelumnya dengan sekali klik
* Fitur hapus riwayat untuk membersihkan data lama

### ⛽ Kalkulator Konsumsi BBM Saat Antri
* Estimasi BBM yang terbuang saat mesin idle di antrian
* Perhitungan biaya BBM yang terbuang
* Tips untuk menghemat BBM dan mengurangi polusi

### 📤 Bagikan Hasil
* Tombol share untuk membagikan hasil perhitungan
* Support native share API (mobile)
* Fallback ke clipboard untuk browser desktop

## 🚀 Demo Aplikasi
Coba langsung aplikasinya di sini:
🔗 **[https://antrianspbu.netlify.app/](https://antrianspbu.netlify.app/)**

## 📸 Screenshots

### Mode Gelap (Dark Theme)
![Mode Gelap](https://github.com/user-attachments/assets/9d424a03-d818-44a5-8208-21838bed2d94)

### Mode Terang (Light Theme)
![Mode Terang](https://github.com/user-attachments/assets/0ce9aa11-9f17-449b-aec8-0570b7153d1c)

### Hasil Perhitungan dengan Fitur Lengkap
![Hasil Lengkap](https://github.com/user-attachments/assets/f2471059-e3e4-403d-827d-d1f1bb462bce)
