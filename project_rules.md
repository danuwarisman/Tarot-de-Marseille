# Panduan Pembuatan Website Tarot (Tugas Kampus)

## 1. Konteks Proyek

Ini adalah tugas kampus pembuatan website statis. Website ini bertema Tarot dengan referensi gaya kartu "Tarot de Marseille".

* **TIDAK BOLEH** menggunakan framework CSS apapun (Tidak boleh Bootstrap, Tailwind, dll).
* **TIDAK BOLEH** menggunakan framework JS (Tidak boleh React, Vue, dll).
* **HANYA** boleh menggunakan murni Vanilla HTML dan murni Vanilla CSS.
* Jika fitur "Ramalan" membutuhkan logika interaktif, gunakan Vanilla JavaScript seminimal mungkin, atau lebih disarankan menggunakan trik interaktivitas murni CSS (seperti *CSS Flip Card* dengan hover atau *checkbox hack*).

## 2. Struktur Navigasi (Minimal 5 Menu)

Website harus memiliki 5 halaman (file `.html` terpisah atau navigasi *single-page* jika diminta, namun disarankan multi-page standar):

1. **Beranda (`index.html`):** Halaman utama, hero section dengan judul besar, kalimat sambutan, dan tombol *Call to Action* "Mulai Ramalan".

2. **Sejarah (`sejarah.html`):** Artikel berformat rapi tentang sejarah Tarot (fokus pada era Renaissance dan Tarot de Marseille).

3. **Arti Kartu (`kartu.html`):** Halaman galeri yang menampilkan gambar-gambar kartu dari folder `card/`. Setiap gambar kartu harus memiliki teks penjelasan maknanya.

4. **Ramalan (`ramalan.html`):** Halaman simulasi "Ambil Satu Kartu" (Card of the Day / Single Draw). Buatlah animasi CSS di mana kartu tertutup, dan saat di-hover/klik akan berputar (flip) menampilkan gambar kartu (misalnya `card/b06.jpg`) dan hasil bacaannya.

5. **Tentang (`tentang.html`):** Halaman profil pembuat website (Tugas Kampus). **Wajib** diisi dengan data pembuat berikut:
   * **Nama:** Danu Warisman
   * **NIM:** 103122400041
   * **Kelas:** S1SE-08-02
   Tambahkan juga paragraf singkat tentang latar belakang pembuatan website ini sebagai tugas kampus.

## 3. Tema dan Panduan Desain (Styling)

Desain harus disesuaikan dengan gambar referensi kartu (Tarot de Marseille - `b06.jpg`).

* **Gaya Visual:** Klasik, elegan, vintage Eropa, bersih (clean), dan terstruktur. Jangan gunakan tema "Dark/Gothic" yang berlebihan.
* **Palet Warna:**
  * **Background Utama:** Putih Tulang / Krem / Parchment (contoh: `#F9F6F0` atau `#FAF0E6`).
  * **Teks Utama:** Hitam pekat atau Abu-abu sangat gelap (contoh: `#1A1A1A`) agar kontras dan mudah dibaca.
  * **Warna Aksen 1 (Primary):** Merah Bata / Merah Klasik (terinspirasi dari warna merah pada kartu, contoh: `#C23B22` atau `#D32F2F`). Gunakan untuk tombol, hover link, atau garis bawah judul.
  * **Warna Aksen 2 (Secondary):** Biru Pucat (contoh: `#8EB8D4`). Gunakan untuk highlight atau background section alternatif.
  * **Warna Aksen 3 (Tertiary):** Kuning Emas (contoh: `#FFD700` atau `#E5A91E`). Gunakan untuk ornamen atau border.
* **Tipografi (Font):**
  * **Heading (H1, H2, H3):** Gunakan font Serif klasik (seperti `Playfair Display`, `Georgia`, atau `Times New Roman`) agar terkesan mistis dan historis.
  * **Body Text (P):** Boleh Serif yang mudah dibaca atau Sans-serif yang bersih (seperti `Lora`, `Merriweather`, atau `Arial/Helvetica` standar).
* **Layout:** Gunakan CSS Flexbox atau CSS Grid untuk mengatur tata letak galeri kartu agar responsif.

## 4. Pengelolaan Aset (Assets)

* Semua file HTML diletakkan di root folder.
* File CSS diletakkan di folder `css/` (misal: `css/style.css`).
* Semua gambar kartu diletakkan di folder `card/`.
* **Penting:** Pastikan path gambar pada tag `<img>` mengarah ke folder yang benar, contoh: `<img src="card/b06.jpg" alt="Kartu Tarot">`.

## 5. Instruksi Khusus untuk AI Agent

Saat Anda (AI) membuat kode untuk website ini, pastikan:

1. Menuliskan struktur HTML5 yang semantik (menggunakan `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`).
2. CSS harus rapi, menggunakan komentar untuk memisahkan bagian (misal: `/* HEADER */`, `/* GALLERY */`).
3. Buatlah transisi (transition) atau animasi CSS yang halus pada tombol dan kartu agar website terasa hidup meskipun tanpa framework.
4. Isi konten berupa teks bahasa Indonesia yang bermakna dan sesuai dengan konteks tarot, serta pastikan halaman "Tentang" diisi dengan data Danu Warisman secara akurat.