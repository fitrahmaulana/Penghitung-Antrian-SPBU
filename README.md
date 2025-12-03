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

## 🚀 Demo Aplikasi
Coba langsung aplikasinya di sini:
🔗 **[https://antrianspbu.netlify.app/](https://antrianspbu.netlify.app/)**

## 📸 Screenshots
![Tampilan Aplikasi](https://raw.githubusercontent.com/fitrahmaulana/Penghitung-Antrian-SPBU/refs/heads/main/preview.png)
