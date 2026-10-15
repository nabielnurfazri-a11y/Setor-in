# Hitung Setoran

Aplikasi web untuk menghitung pendapatan kotor, setoran ke tiap penyetor, biaya operasional, dan uang bersih harian. Bisa dipasang di layar utama HP dan jalan tanpa internet.

## Isi folder

| File | Fungsi |
|---|---|
| `index.html` | Seluruh aplikasi |
| `manifest.webmanifest` | Data agar bisa dipasang di layar utama |
| `sw.js` | Service worker, supaya bisa dipakai offline |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | Ikon aplikasi |

Semua file harus berada di folder yang sama (tanpa subfolder).

## Cara pasang di GitHub Pages

1. Buka github.com, masuk, lalu buat repository baru (misalnya `hitung-setoran`), pilih Public.
2. Di repository itu pilih **Add file > Upload files**, unggah semua 6 file di atas, lalu **Commit changes**.
3. Buka **Settings > Pages**. Di bagian *Build and deployment*, pilih Source **Deploy from a branch**, branch **main**, folder **/ (root)**, lalu **Save**.
4. Tunggu 1 sampai 2 menit. Alamat aplikasi akan muncul di halaman yang sama: `https://NAMAKAMU.github.io/hitung-setoran/`

## Pasang di layar utama HP

- **Android (Chrome):** buka alamatnya, ketuk menu titik tiga, pilih **Instal aplikasi** atau **Tambahkan ke layar utama**.
- **iPhone (Safari):** ketuk tombol Bagikan, lalu **Tambah ke Layar Utama**.

## Memindahkan data dari versi Claude

Data tersimpan di browser dan tidak ikut pindah otomatis. Di versi lama buka tab **Atur**, ketuk **Unduh Cadangan Data**. Di aplikasi baru buka tab **Atur**, ketuk **Pulihkan Data**, lalu pilih file cadangan itu.

## Mengubah aplikasi nanti

Ganti `index.html` di repository, lalu naikkan angka versi di `sw.js` (misalnya `hitung-setoran-v2`) supaya HP mengambil versi terbaru.

## Catatan

- Data tersimpan di localStorage browser per perangkat. Kalau cache atau data situs dihapus, data hilang, jadi unduh cadangan secara berkala.
- Tombol "Cetak Struk" memakai fitur cetak browser dengan lebar kertas 58 mm.
