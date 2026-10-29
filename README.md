# HP Cayra – AU iPhone Simulator

Simulasi HP iPhone untuk AU dari sudut pandang Cayra. Satu halaman web, tanpa framework, tanpa build.

**Demo:** https://kimwoomens2u-design.github.io/hp-cayra/
**Kode sandi layar kunci:** `202508`

## Fitur
- Layar kunci dengan notifikasi dan kode sandi 6 digit, lalu layar utama dengan 2 halaman (geser ke samping), widget cuaca dan kalender
- **WhatsApp** – daftar chat, 20+ kontak dan grup, chat `mnyt🐵` yang mengetik pesan baru secara live, profil kontak
- **Instagram** – feed, story bergambar, profil, komentar, DM (termasuk dari akun anonim dan fans)
- **X (Twitter)** – dua akun (publik dan gembokan), timeline, notifikasi, DM, posting tweet
- **Spotify** – daftar lagu Hearts2Hearts, pemutar penuh (acak, ulang, geser durasi)
- **Foto, Kamera, Pesan lain** – galeri dengan wallpaper, kamera selfie, Telepon, Safari (simulasi), Mail, Catatan, Pengingat, Jam, Kalender, Peta, Kesehatan, Dompet, App Store, Pengaturan, Kalkulator, Cuaca, Roblox

## Struktur folder
Semua file ada langsung di folder utama (tanpa subfolder), jadi gampang diupload lewat web GitHub.

| File | Fungsi |
|---|---|
| `index.html` | Seluruh aplikasi (HTML + CSS + JavaScript) |
| `.nojekyll` | Supaya GitHub Pages menyajikan file apa adanya |
| `wallpaper-layar-kunci.jpg`, `wallpaper-layar-utama.jpg` | Wallpaper layar kunci dan layar utama |
| `instagram.png`, `x.png`, `whatsapp.png`, `spotify.png`, `roblox.png` | Ikon aplikasi |
| `foto-formal.jpg`, `backstage.jpg`, `dinner.jpg`, `pantai-malam.jpg`, `jaket-kulit.jpg`, `pita-hutan.jpg`, `temen-di-semak.jpg`, `topi-overall.jpg` | Postingan dan galeri Cay.Ra_ |
| `stayz-1.jpg` … `stayz-6.jpg`, `yuebi-1.jpg` … `yuebi-4.jpg`, `hearts2hearts-1.jpg` … `-5.jpg`, `jisoo-1.jpg`, `jyandcs-1.jpg` | Postingan di feed akun lain |
| `mnyt.jpg`, `prem.jpg`, `stayz-wa.jpg`, `yuebi-wa.jpg` | Foto profil WhatsApp / DM |
| `stayz-ig-profil.jpg`, `yuebi-ig-profil.jpg`, `*-ig-lama.jpg`, `jisoo-ig-profil.jpg`, `hearts2hearts-logo.jpg`, `band-profil.jpg`, `mua-profil.jpg` | Foto profil Instagram |
| `*-story.jpg` (mis. `cayra-story.jpg`, `stayz-story-kafe.jpg`) | Gambar story |
| `karhutla-*.jpg`, `kabut-asap-anak.jpg`, `berita-hujan.jpg`, `bicara-lantang.jpg`, `suara-rakyat.jpg`, `kucing.jpg`, `makeup-kit.jpg`, `ruang-rias.jpg`, `dapur.jpg`, `konser.jpg` | Gambar postingan akun lain |

## Pasang di GitHub Pages
1. Buat repository baru (Public), mis. `hp-cayra`.
2. **Add file → Upload files**, pilih **semua file** di folder ini (Ctrl+A) lalu seret. Batas upload web 100 file per kali. Klik **Commit changes**.
3. **Settings → Pages → Deploy from a branch → main / (root) → Save**.
4. Tunggu 1–2 menit, buka `https://USERNAME.github.io/hp-cayra/`.
5. Kalau tampilan belum berubah setelah update, refresh keras dengan Ctrl+Shift+R.

## Mengganti foto
Timpa file dengan foto baru **bernama sama** (`.jpg` tetap `.jpg`, `.png` tetap `.png`). Kalau mau menambah foto baru, taruh di folder utama lalu panggil namanya di `index.html`.

## Mengubah isi chat, DM, komentar, dan X
Buka `index.html`, tekan Ctrl+F lalu cari:
- WhatsApp: `const C=` dan `addC(`
- DM Instagram: `const DM=` dan `const DTH=`
- Komentar Instagram: `const CM=` · feed Instagram: `const FP=`
- Aplikasi X: `const XL=` (tweet), `const XA=` (akun), `const XM=` (DM)

Format pesan: `m|teks` (lawan bicara) · `a|teks` (Cayra) · `t|16.32` (penanda jam) · `x|teks` (info sistem).

Hati-hati: setiap pesan harus diapit tanda kutip `'...'` dan dipisah koma. Tanda kutip yang hilang akan membuat seluruh halaman tidak jalan.

## Musik (Hearts2Hearts)
Daftar lagu sudah terisi, tetapi file audionya tidak disertakan. Taruh mp3 milikmu di **folder utama** dengan nama persis seperti ini:

`the-chase.mp3`, `butterflies.mp3`, `style.mp3`, `pretty-please.mp3`, `focus.mp3`, `apple-pie.mp3`, `flutter.mp3`, `blue-moon.mp3`, `rude.mp3`, `lemon-tang.mp3`, `15-love.mp3`, `baby-steps.mp3`, `heart-emoji.mp3`, `secret-recipe.mp3`

Kalau file belum ada, ketuk ikon ⤒ di samping judul lagu untuk memilih mp3 dari perangkat (hanya berlaku selama halaman terbuka).

## Catatan
- Ini karya fiksi (AU). Semua nama, chat, dan akun adalah rekaan.
- Kamera butuh izin browser dan hanya jalan lewat HTTPS (GitHub Pages sudah HTTPS).
