# MINPRO 1 Pemrograman Berbasis Web
Nama: Indah Putri Lestari

NIM: 2409116004

Kelas: A'2024

# Deskripsi Project Website Portfolio – Indah Putri Lestari

Project ini merupakan website portfolio sederhana berbasis HTML dan CSS dengan tambahan Bootstrap 5 dan Vue JS untuk mendukung layout serta interaktivitas ringan.

Website terdiri dari tiga section utama:
- Home
- About Me
- Certificates

Website bersifat statis karena tidak menggunakan database maupun backend.

# Struktur File

<img width="399" height="613" alt="image" src="https://github.com/user-attachments/assets/c620a51e-c4b6-44d4-b93e-7f5ecaa9229c" />

# Tampilan dan Penjelasan Code Setiap Section / Fitur

## 1. Navbar

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/2dfaf066-81ab-4b03-a8b9-4064b0943ca4" />

**Penjelasan Code**

Navbar dibuat menggunakan komponen dari Bootstrap 5 dengan class `navbar`, `navbar-expand-lg`, dan `fixed-top`. Struktur ini memungkinkan navbar tampil responsif serta tetap berada di bagian atas halaman ketika pengguna melakukan scroll.

Judul website ditempatkan pada bagian kiri menggunakan class `navbar-brand`, sedangkan menu navigasi seperti `Home`, `About Me`, dan `Certificates` diletakkan di sisi kanan menggunakan `navbar-nav` dan `nav-item`. Setiap menu menggunakan anchor link seperti `href="#home"` yang berfungsi untuk mengarahkan pengguna ke section tertentu dalam satu halaman yang sama.

Tampilan warna latar, bayangan, serta penyesuaian jarak memanfaatkan kombinasi class Bootstrap dan pengaturan tambahan pada file `style.css` agar tetap selaras dengan tema desain website.

## 2. Home (Hero Section)

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/64c62cfa-dd82-4345-8c5e-c787dacf4d29" />

**Penjelasan Code**

Section ini dibuat menggunakan elemen `<section id="home">` sebagai tampilan pembuka website. Tata letak memanfaatkan class Bootstrap seperti `container`, `d-flex`, `align-items-center`, dan `text-center` sehingga seluruh konten dapat diposisikan di tengah layar secara horizontal dan vertikal.

Nama ditampilkan menggunakan Vue JS dengan interpolation `{{ name }}`. Data tersebut didefinisikan di dalam fungsi `data()` dan dihubungkan ke elemen utama menggunakan `.mount('#app')`. Pendekatan ini memungkinkan pengelolaan data secara terstruktur meskipun website tetap bersifat statis.

Foto profil ditampilkan menggunakan elemen `<img>` dan diberi styling pada file `style.css` seperti `border-radius: 50%` untuk membentuk lingkaran serta `box-shadow` untuk memberikan efek bayangan. Latar belakang section diatur menggunakan properti `linear-gradient` agar tampilan lebih menarik.

Tombol “Explore More” menggunakan class `btn` dari Bootstrap dan dikombinasikan dengan class kustom `btn-purple` untuk menyesuaikan warna dengan tema utama website. Tombol tersebut menggunakan `href="#about"` untuk mengarahkan pengguna ke section berikutnya.

## 3. About Me

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/68637b59-65d0-470b-8939-5ae6c88ed6cf" />

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/c9ac8c49-ed74-4476-b22f-0383ea6a63a7" />

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/3b09fc00-e32b-4627-b5b8-193717dcb1b5" />

**Penjelasan Code**

Section ini dibangun menggunakan elemen `<section id="about">` sebagai struktur utama untuk menampung seluruh informasi profil. Tata letaknya memanfaatkan sistem grid Bootstrap seperti `container`, `row`, dan `col-md-6` sehingga konten dapat dibagi menjadi dua bagian yang seimbang dan tetap menyesuaikan ukuran layar.

Bagian deskripsi diri dan tujuan karier ditempatkan dalam satu baris dengan pembagian kolom yang berbeda. Penyusunan ini bertujuan agar informasi utama dan visi profesional dapat ditampilkan secara berdampingan tanpa terlihat padat. Elemen “Tujuan Karier” diberikan penegasan visual melalui pengaturan pada file `style.css`, seperti garis vertikal di sisi kiri serta penyesuaian jarak dalam elemen agar tampil lebih menonjol.

Daftar Pengalaman & Aktivitas disusun menggunakan elemen `<ul>` yang dipadukan dengan ikon dari Bootstrap Icons sehingga setiap poin memiliki penanda visual yang jelas. Untuk bagian Pendidikan, digunakan pengaturan flexbox agar ikon dan teks dapat tersusun sejajar secara horizontal sehingga tampilan lebih terstruktur.

Pada bagian Skills, digunakan komponen `progress` dan `progress-bar` dari Bootstrap untuk menampilkan tingkat kemampuan dalam bentuk persentase. Nilai lebar setiap bar ditentukan melalui atribut `data-width`, kemudian dijalankan animasinya menggunakan JavaScript saat halaman di-scroll.

Seluruh pengaturan warna, tipografi, jarak antar elemen, garis pemisah, efek bayangan, serta penyesuaian responsif diatur pada file `style.css` dengan memanfaatkan variabel warna pada `:root`, properti CSS, dan media query.

## 4. Certificates

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/d618401e-9156-4e1f-89fc-679d06e5c844" />

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/21ccf6a7-7625-40ef-9b0e-3d21f6c0232b" />

**Penjelasan Code**

Section ini dibuat menggunakan elemen `<section id="certificates">` sebagai wadah untuk menampilkan daftar sertifikat. Penyusunan konten memanfaatkan sistem grid Bootstrap seperti `container`, `row`, dan `col-md-4` sehingga setiap sertifikat ditampilkan dalam bentuk kolom yang tersusun rapi dan tetap responsif pada berbagai ukuran layar.

Data sertifikat tidak dituliskan langsung secara manual di dalam struktur HTML, melainkan disimpan dalam array pada bagian `data()` di Vue JS. Setiap objek di dalam array memuat properti `title`, `year`, dan `image`. Data tersebut kemudian ditampilkan menggunakan directive `v-for`, sehingga setiap item secara otomatis dirender menjadi satu card tanpa perlu menuliskan struktur berulang.

Struktur card menggunakan komponen Bootstrap dengan class `card` dan `card-body` untuk menjaga konsistensi tampilan. Gambar sertifikat dihubungkan menggunakan binding Vue `:src="cert.image"` sehingga sumber gambar mengikuti data yang telah didefinisikan pada array.

Efek interaktif pada card diatur melalui file `style.css` dengan memanfaatkan properti `transform: translateY(-8px);` serta `transition` agar pergerakan saat hover terlihat halus. Selain itu, pengaturan warna latar, sudut membulat, serta bayangan ditentukan melalui CSS guna mempertahankan keselarasan dengan tema keseluruhan website.

# Teknologi yang Digunakan

## 1. HTML

Digunakan untuk membangun struktur dasar website, seperti membuat navbar, section (Home, About Me, Certificates), menampilkan teks, gambar, tombol, serta mengatur susunan elemen pada halaman.

## 2. CSS

Digunakan untuk mengatur tampilan dan desain website, seperti warna, background, font, jarak antar elemen, layout, efek bayangan, serta animasi sederhana agar tampilan lebih menarik dan rapi.

## 3. Bootstrap 5

Digunakan untuk membantu proses layout dan styling dengan lebih cepat, seperti penggunaan grid system (container, row, col), navbar, card, button, progress bar, serta mendukung desain yang responsif di berbagai ukuran layar.

## 4. Bootstrap Icons

Digunakan untuk menambahkan ikon pada bagian pengalaman dan pendidikan agar tampilan lebih informatif dan menarik.

## 5. Vue JS

Digunakan untuk menampilkan data secara interaktif menggunakan interpolation ({{ }}), directive v-for, serta struktur data() dan .mount('#app'), meskipun data yang digunakan tetap bersifat statis.
