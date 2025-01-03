# MovieTime App

## Deskripsi

Aplikasi cerdas yang memberikan rekomendasi film personal berdasarkan model Deep Learning. Dengan fitur ulasan (review) film, MovieTime mempelajari preferensi pengguna untuk memberikan rekomendasi yang lebih akurat dan sesuai selera Anda.

---

## Prasyarat

Sebelum menjalankan aplikasi ini anda perlu menjalankan API Service terlebih dahulu, Backend Service untuk aplikasi ini berada di repository yang terpisah:
[MovieTime App Backend Services](https://github.com/raparsalan/movietime-backend)

Sebelum menjalankan aplikasi ini, pastikan Anda telah menginstal **ADB (Android Debug Bridge)**. ADB diperlukan untuk menghubungkan perangkat Android dengan komputer Anda selama proses pengembangan dan debugging.

### Langkah-Langkah Instalasi ADB

1. **Download Android SDK Platform Tools**:

   - Anda dapat mengunduhnya dari [Android Developer Official Website](https://developer.android.com/studio/releases/platform-tools).

2. **Ekstrak File**:

   - Setelah diunduh, ekstrak file `platform-tools` ke lokasi pilihan Anda (misalnya: `C:\platform-tools`).

3. **Tambahkan ke PATH (Opsional, tapi Direkomendasikan)**:

   - Tambahkan direktori `platform-tools` ke variabel lingkungan `PATH` agar Anda dapat menjalankan perintah ADB dari terminal mana saja.

4. **Verifikasi Instalasi**:
   - Buka terminal/command prompt dan jalankan perintah:
     ```bash
     adb --version
     ```
   - Jika berhasil, Anda akan melihat versi ADB yang terinstal.

### Setting Port pada ADB

Karena Backend Service berjalan di localhost:5000 maka device android perlu mengetahui hal tersebut, untuk itu perlu menjalankan command berikut:

```bash
    adb reverse tcp:5000 tcp:5000
```

## Menjalankan Aplikasi

1. **Akses Halaman Release**:

   - Buka tab **[Releases](https://github.com/rifqifajarr/movietime/releases/tag/v1.0.0)** di repository ini.

2. **Unduh APK**:

   - Cari versi terbaru yang tersedia di halaman **Releases**.
   - Klik pada file `.apk` untuk memulai proses unduhan.

3. **Izinkan Instalasi dari Sumber Tidak Dikenal**:

   - Sebelum menginstal APK, pastikan Anda telah mengaktifkan opsi **"Install from Unknown Sources"** di perangkat Android Anda.
   - Cara mengaktifkannya:
     - Masuk ke **Settings** > **Security** > Aktifkan **Unknown Sources** (Sumber Tidak Dikenal).

4. **Instal APK**:

   - Setelah unduhan selesai, buka file APK dari folder unduhan perangkat Anda.
   - Klik **Install** untuk memulai instalasi.

5. **Jalankan Aplikasi**:
   - Setelah proses instalasi selesai, Anda dapat membuka aplikasi langsung dari perangkat Anda.
