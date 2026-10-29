# HP Cayra – AU iPhone Simulator

Simulasi HP iPhone untuk AU dari sudut pandang Cayra. Satu halaman web, tanpa framework.
**Kode sandi layar kunci: `202508`**

## Isi folder
- `index.html` – seluruh aplikasi (HTML + CSS + JavaScript)
- `assets/` – semua gambar (postingan, foto profil, story, wallpaper, ikon)
- `songs/` – taruh file mp3 di sini

## Pasang di GitHub Pages
1. Buat repository baru (Public), mis. `hp-cayra`.
2. **Add file → Upload files**, seret SEMUA isi folder ini, lalu **Commit changes**.
3. **Settings → Pages → Deploy from a branch → main / (root) → Save**.
4. Tunggu 1–2 menit: `https://USERNAME.github.io/hp-cayra/`

## Mengganti foto
Timpa file di `assets/` dengan foto baru **bernama sama** (.jpg).
`assets/akun/` = foto profil & story akun · `assets/cayra/` = postingan Cay.Ra_ · `assets/timeline/` = postingan akun lain · `assets/wallpaper-layar-kunci.jpg` = wallpaper layar kunci · `assets/wallpaper-layar-utama.jpg` = wallpaper layar aplikasi

## Mengubah isi chat / DM / komentar / X
Buka `index.html`, tekan Ctrl+F:
- WhatsApp: `const C=` dan `addC(` · DM Instagram: `const DM=` dan `const DTH=`
- komentar Instagram: `const CM=` · feed Instagram: `const FP=`
- aplikasi X: `const XD=` (tweet) dan `const XA=` (akun)
Format pesan: `m|teks` (lawan bicara) · `a|teks` (Cayra) · `t|16.32` (jam) · `x|teks` (info sistem)

## Musik (Hearts2Hearts)
Daftar lagu sudah terisi, tetapi file audionya tidak disertakan. Taruh mp3 milikmu di folder `songs/` dengan nama persis seperti ini:
`the-chase.mp3`, `butterflies.mp3`, `style.mp3`, `pretty-please.mp3`, `focus.mp3`, `apple-pie.mp3`, `flutter.mp3`, `blue-moon.mp3`, `rude.mp3`, `lemon-tang.mp3`, `15-love.mp3`, `baby-steps.mp3`, `heart-emoji.mp3`, `secret-recipe.mp3`
Kalau file belum ada, ketuk ikon ⤒ di samping judul lagu untuk memilih mp3 dari perangkat (hanya berlaku selama halaman terbuka).
