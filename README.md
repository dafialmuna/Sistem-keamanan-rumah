# Sistem Keamanan Rumah dengan ESP32-CAM

Proyek Sistem Keamanan Rumah Pintar menggunakan ESP32-CAM, Sensor PIR, dan Bot Telegram. Proyek ini akan mendeteksi pergerakan dan secara otomatis mengirimkan foto langsung ke Telegram Anda.

## Persiapan Kode

Agar kode ini bisa berjalan dan terhubung ke WiFi serta Telegram Anda, ikuti langkah berikut:

1. Di folder proyek ini, cari file bernama `secrets_dummy.h`.
2. Ubah nama file tersebut (Rename) menjadi `secrets.h`.
3. Buka file `secrets.h` dan masukkan pengaturan Anda sendiri:
   - `ssid`: Isi dengan nama WiFi Anda.
   - `password`: Isi dengan password WiFi Anda.
   - `botToken`: Isi dengan Token Bot Telegram dari BotFather.
   - `chatID`: Isi dengan ID Telegram Anda (dari akun IDBot).
4. Setelah itu, Anda bisa melakukan *Upload* kode `CameraWebServer.ino` ke ESP32-CAM menggunakan Arduino IDE.

**Catatan Keamanan:** File `secrets.h` sudah dimasukkan ke dalam `.gitignore`, sehingga password asli Anda tidak akan pernah terunggah secara tidak sengaja ke GitHub!
