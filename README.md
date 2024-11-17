# SEMANTIC-HTML
Latihan Praktikum SEMANTIC HTML

# Kekurangan dalam HTML
Struktur <section> Tidak Sesuai Konteks

Masalah: Elemen <section> hanya berisi teks placeholder "Konten".
Dampak: Tidak memberikan informasi yang jelas dan tidak memanfaatkan elemen semantik dengan optimal.
Solusi: Tambahkan ID dan konten yang relevan untuk mencerminkan fungsi setiap bagian, seperti berikut:
html
# Perbaikan kode
```
<section id="home">
    <h2>Beranda</h2>
    <p>Selamat datang di panduan HTML5 semantik.</p>
</section>
<section id="pengertian">
    <h2>Pengertian</h2>
    <p>HTML5 adalah versi terbaru dari HTML yang mendukung elemen semantik.</p>
</section>
<section id="kesimpulan">
    <h2>Kesimpulan</h2>
    <p>Penggunaan elemen semantik dapat meningkatkan struktur dan aksesibilitas web.</p>
</section>
```

# Kurangnya Tag Semantik Tambahan
Masalah: Elemen seperti <article> atau <aside> tidak digunakan untuk menambah nilai semantik pada halaman.
Dampak: Halaman kurang terstruktur secara semantik, terutama untuk konten yang membutuhkan pengelompokan lebih baik.
Solusi: Tambahkan elemen semantik jika relevan, misalnya:
html
# Perbaikan kode
```
<article>
    <h3>Manfaat Elemen Semantik</h3>
    <p>Elemen semantik membantu SEO dan meningkatkan pengalaman pengguna.</p>
</article>
```
# Kekurangan dalam CSS
# Warna Tidak Konsisten

Masalah: Warna latar belakang untuk elemen seperti nav, header, dan footer kurang harmonis, sehingga halaman terlihat kurang menarik.
Dampak: Membuat desain tampak kurang profesional.
Solusi: Gunakan skema warna yang konsisten dan sesuai prinsip desain. Misalnya:
css
```
Perbaikan kode
nav {
    background: #8E8E8E; /* Warna seragam dengan elemen lainnya */
}
```
# Navigasi Tidak Fleksibel

Masalah: Navigasi (<nav>) memiliki area kecil (20%) dan kurang responsif untuk perangkat dengan ukuran layar kecil.
Dampak: Navigasi menjadi sulit digunakan pada layar kecil.
Solusi: Tambahkan media query untuk menyesuaikan ukuran nav pada perangkat kecil. Contoh:
css
# Perbaikan kode
```
@media (max-width: 768px) {
    body {
        grid-template-areas:
            "header"
            "nav"
            "section"
            "footer";
        grid-template-rows: 80px auto 1fr 50px;
        grid-template-columns: 1fr;
    }
    nav {
        text-align: center;
    }
}
```
# Elemen Tidak Sepenuhnya Responsif

Masalah: Tampilan section terlalu statis karena hanya mengandalkan grid tanpa fleksibilitas tambahan.
Dampak: Ketika layar berubah, distribusi area mungkin terlihat tidak proporsional.
Solusi: Tambahkan properti min-height atau max-width untuk menjaga proporsi. Contoh:
css
# Perbaikan kode
```
section {
    min-height: 300px;
    padding: 20px;
}
```
# Jarak Antar Elemen Kurang

Masalah: grid-gap: 5px memberikan jarak terlalu kecil antar elemen, terutama untuk layar besar.
Dampak: Membuat desain terlihat padat dan tidak nyaman dipandang.
Solusi: Tingkatkan jarak antar elemen. Contoh:
css
# Perbaikan kode
```
body {
    grid-gap: 10px;
}
```
# Tipografi Belum Optimal

Masalah: Tidak ada pengaturan font yang jelas untuk elemen teks.
Dampak: Teks mungkin terlihat monoton dan sulit dibaca pada perangkat tertentu.
Solusi: Tambahkan aturan font. Contoh:
css
# Perbaikan kode
```
body {
    font-family: Arial, sans-serif;
    font-size: 16px;
    line-height: 1.5;
}
```
