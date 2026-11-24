# Browser Mengambang (Floating Browser)

Aplikasi Android yang membuka browser kecil melayang di atas game atau aplikasi apa pun.

## Fitur
- **Geser**: tarik bar gelap di bagian atas jendela.
- **Ubah ukuran**: tarik sudut kanan-bawah (◢).
- **Transparan**: tombol ◐ (100% → 75% → 50% → 30%).
- **Minimize**: tombol – jadi bubble 🌐; ketuk bubble untuk membuka lagi (bubble juga bisa digeser).
- **Mode ketik**: tombol ⌨. Aktifkan kalau mau mengetik di halaman web. Saat mati, jendela tidak
  mengambil fokus sehingga game di belakang tetap jalan normal.
- Bar alamat: ketik URL atau kata kunci pencarian, lalu tekan Go.
- Tutup: tombol ✕ atau tombol "Hentikan" di notifikasi.

## Cara build

### Opsi A: Android Studio
1. Buka Android Studio → **Open** → pilih folder `FloatingBrowser`.
2. Tunggu Gradle sync selesai (butuh internet, pertama kali agak lama).
3. Colok HP (USB debugging aktif) → tekan **Run**. Atau **Build > Build APK(s)** lalu pasang APK-nya.

### Opsi B: Tanpa Android Studio (cocok untuk laptop RAM kecil)
1. Buat repo di GitHub, upload seluruh isi folder ini.
2. Buka tab **Actions** → **Build APK** → **Run workflow**.
3. Setelah selesai, unduh artifact `app-debug` → di dalamnya ada `app-debug.apk`.
4. Pasang di HP (izinkan "Install dari sumber tidak dikenal").

## Cara pakai
1. Buka aplikasi → tekan **Beri izin overlay** → aktifkan "Tampilkan di atas aplikasi lain".
2. Tekan **Mulai browser mengambang**.
3. Buka game/aplikasi lain; jendela browser tetap melayang di atasnya.

## Catatan
- Aplikasi ini hanya menampilkan jendela browser di atas aplikasi lain. Tidak mengubah isi game.
- Sebagian game memblokir overlay atau pause saat jendela lain mengambil fokus; itu perilaku game-nya.
- Di Android 12+, tingkat transparan ≤ 75% membantu supaya sentuhan ke app di belakang tidak diblokir.
