# 🚀 Kaspa (KAS) Breakout Alert Page

Halaman web sederhana berbasis HTML + JavaScript untuk **memantau harga Kaspa (KAS)** secara real-time dan memberikan **alert otomatis saat terjadi breakout** di atas level resistance tertentu.

---

## 📌 Fitur

- Cek harga KAS setiap 60 detik via [CoinGecko API](https://www.coingecko.com/)
- Menampilkan harga real-time di halaman browser
- Log historis harga + waktu
- Alert otomatis via popup browser saat harga tembus resistance (default: `$0.205`)
- Desain dark mode minimalis

---

## 📁 Struktur File

- `index.html` – Halaman utama + script monitor
- Tidak membutuhkan file eksternal tambahan

---

## 🚀 Cara Menggunakan

1. **Download / Salin file `index.html`**
2. Buka file tersebut di browser modern (Chrome, Firefox, Edge)
3. Biarkan terbuka untuk memantau harga
4. Jika harga KAS menembus level breakout, alert popup akan muncul

---

## ⚙️ Konfigurasi

Di dalam `<script>`:

```js
const resLevel = 0.20;   // Level resistance utama
const alertLvl = 0.205;  // Harga untuk trigger alert (~2.5% di atas resistance)
const cooldown = 30 * 60 * 1000; // 30 menit antara alert
