# KIOS QIEL PWA

Paket siap diunggah ke GitHub Pages. Aplikasi menggunakan penyimpanan lokal browser (`localStorage`) untuk data kasir; data tidak otomatis tersinkron ke perangkat lain.

## Isi paket
- `index.html` — aplikasi kasir KIOS QIEL dengan keranjang pop-up.
- `manifest.webmanifest` — metadata instalasi PWA.
- `sw.js` — cache app shell untuk membuka aplikasi saat offline setelah kunjungan online pertama.
- `icons/` — ikon PWA ukuran 192×192 dan 512×512, termasuk maskable.
- `README.md` — panduan.

## Cara unggah ke GitHub Pages dari HP
1. Unduh lalu ekstrak `KIOS_QIEL_PWA.zip`.
2. Buka repositori: https://github.com/renelumapow31-dev/Kios-Qiel-PWA
3. Pilih **Add file → Upload files**.
4. Unggah semua ISI folder ini (bukan file ZIP): `index.html`, `manifest.webmanifest`, `sw.js`, folder `icons`, dan `README.md`.
5. Tekan **Commit changes**.
6. Buka **Settings → Pages**. Pilih **Deploy from a branch**, branch `main`, folder `/(root)`, lalu **Save**.
7. Setelah deployment selesai, buka https://renelumapow31-dev.github.io/Kios-Qiel-PWA/ melalui Chrome Android.
8. Buka menu Chrome **⋮ → Tambahkan ke layar utama** atau **Install app** jika tersedia.

## Setelah pembaruan
Service worker dapat menyimpan versi lama sementara. Tutup aplikasi, buka ulang saat online, dan jika perlu buka Chrome → Info situs → Penyimpanan → hapus data situs. Perhatian: menghapus data situs dapat menghapus data kasir lokal yang belum dicadangkan.

## Catatan penting
- PWA membutuhkan HTTPS; GitHub Pages menyediakan HTTPS.
- Dukungan offline app shell aktif setelah halaman berhasil dimuat online pertama kali. Fitur khusus browser (misalnya cetak dan pemilih folder cadangan) tetap mengikuti dukungan browser.
- Data `localStorage` hanya berada di browser/perangkat yang sama. Cadangkan data secara berkala.
- Paket ini telah diperiksa sintaks JavaScript dasar, tetapi belum diuji langsung pada perangkat Android. Sebelum dipakai untuk transaksi sungguhan, uji tambah produk, pembayaran Cash/Transfer, laporan, backup/restore, refresh, pemasangan, dan mode pesawat.
