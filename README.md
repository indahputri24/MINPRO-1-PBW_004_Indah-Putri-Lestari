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

**a. Tampilan**

Pada bagian paling atas website terdapat navbar dengan latar belakang putih dan bayangan tipis. Navbar ini menampilkan judul “Portfolio Indah Putri Lestari” di sebelah kiri serta menu navigasi Home, About Me, dan Certificates di sebelah kanan. Navbar bersifat tetap (fixed) di bagian atas sehingga tetap terlihat saat halaman di-scroll.
  
**b. Penjelasan Code**

Navbar dibuat menggunakan komponen dari Bootstrap 5 dengan class `navbar`, `navbar-expand-lg`, dan `fixed-top`. Menu navigasi menggunakan anchor link seperti `href="#home"` yang berfungsi untuk mengarahkan pengguna ke section tertentu dalam satu halaman yang sama. Tampilan warna dan bayangan tambahan diatur menggunakan class Bootstrap dan CSS pada file `style.css`.

## 2. Home (Hero Section)

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/64c62cfa-dd82-4345-8c5e-c787dacf4d29" />

**a. Tampilan**
  
Section Home merupakan tampilan pembuka website. Bagian ini menampilkan foto profil berbentuk lingkaran, nama lengkap, NIM, deskripsi singkat, serta tombol “Explore More”. Latar belakang menggunakan gradasi warna ungu dan pink sehingga tidak monoton. Seluruh isi section diposisikan di tengah layar agar terlihat rapi dan seimbang.

**b. Penjelasan Code**

Section ini dibuat menggunakan elemen `<section id="home">` dan memanfaatkan layout Bootstrap seperti `container`, `d-flex`, dan `align-items-center` untuk mengatur posisi konten. Nama ditampilkan menggunakan Vue JS dengan interpolation `{{ name }}` yang datanya didefinisikan di dalam `data()` dan dihubungkan ke elemen menggunakan `.mount('#app')`. Styling seperti background gradient, bentuk lingkaran pada foto, serta warna tombol diatur dalam file `style.css`.

## 3. About Me

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/68637b59-65d0-470b-8939-5ae6c88ed6cf" />

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/c9ac8c49-ed74-4476-b22f-0383ea6a63a7" />

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/3b09fc00-e32b-4627-b5b8-193717dcb1b5" />

**a. Tampilan**

Section About Me menampilkan informasi lengkap mengenai profil diri. Bagian ini dibungkus dalam sebuah container berwarna putih dengan sudut membulat dan bayangan halus sehingga terlihat seperti card besar di atas background.

Di bagian atas terdapat judul “About Me” dengan garis dekoratif di bawahnya sebagai elemen visual. Setelah itu ditampilkan deskripsi diri yang menjelaskan latar belakang pendidikan, minat di bidang teknologi dan bisnis, serta keaktifan dalam mengikuti pelatihan dan kegiatan pengembangan diri.

Di sisi kanan deskripsi terdapat bagian “Tujuan Karier” yang ditampilkan dalam bentuk box dengan garis vertikal berwarna ungu sebagai aksen. Bagian ini menonjolkan tujuan profesional secara singkat dan jelas.

Di bawahnya, konten dibagi menjadi dua kolom. Kolom kiri berisi Pengalaman & Aktivitas dalam bentuk daftar dengan ikon bintang, sedangkan kolom kanan berisi Pendidikan yang dilengkapi ikon dan informasi tahun. Pada bagian paling bawah terdapat Skills yang ditampilkan menggunakan progress bar untuk menunjukkan tingkat kemampuan.

**b. Penjelasan Code**

Section ini dibuat menggunakan elemen `<section id="about">` dan memanfaatkan sistem grid dari Bootstrap seperti `container`, `row`, dan `col-md-6` untuk membagi konten menjadi beberapa bagian. Layout dua kolom memungkinkan informasi tersusun lebih terstruktur dan responsif ketika diakses melalui perangkat berbeda.

Bagian deskripsi dan tujuan karier dibuat dalam satu baris dengan dua kolom berbeda. Elemen “Tujuan Karier” diberi styling khusus pada file `style.css`, seperti border kiri berwarna ungu dan padding tambahan untuk memberikan penekanan visual.

Daftar Pengalaman & Aktivitas dibuat menggunakan elemen `<ul>` dengan ikon dari Bootstrap Icons untuk memperjelas tampilan setiap poin. Sementara itu, bagian Pendidikan menggunakan struktur flexbox agar ikon dan teks dapat sejajar secara horizontal.

Pada bagian Skills, progress bar menggunakan komponen Bootstrap dengan class `progress` dan `progress-bar`. Lebar setiap bar diatur menggunakan atribut `data-width` dan dianimasikan melalui JavaScript ketika pengguna melakukan scroll. Hal ini memberikan efek interaktif meskipun website tetap bersifat statis.

Seluruh warna, jarak antar elemen, efek bayangan, garis pemisah, serta tampilan responsif diatur dalam file `style.css` menggunakan variabel warna pada `:root`, media query, dan properti CSS lainnya.

## 4. Certificates

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/d618401e-9156-4e1f-89fc-679d06e5c844" />

<img width="3200" height="2000" alt="image" src="https://github.com/user-attachments/assets/21ccf6a7-7625-40ef-9b0e-3d21f6c0232b" />

**a. Tampilan** 

Section Certificates menampilkan daftar sertifikat yang dimiliki dalam bentuk card yang tersusun rapi menggunakan layout grid. Pada bagian atas terdapat judul “Certificates” yang diposisikan di tengah halaman. 

Setiap sertifikat ditampilkan dalam bentuk card yang berisi gambar sertifikat, judul kegiatan, dan tahun pelaksanaan. Card memiliki sudut membulat serta bayangan halus agar terlihat lebih modern. Ketika kursor diarahkan ke card, muncul efek hover berupa pergerakan sedikit ke atas sehingga memberikan kesan interaktif.

**b.Penjelasan Code**

Section ini dibuat menggunakan elemen `<section id="certificates">` dan memanfaatkan sistem grid Bootstrap seperti `container`, `row`, dan `col-md-4` untuk mengatur tata letak card dalam bentuk kolom.

Data sertifikat tidak ditulis langsung satu per satu di dalam HTML, tetapi disimpan dalam array pada bagian `data()` di Vue JS. Setiap objek dalam array berisi properti `title`, `year`, dan `image`. Data tersebut kemudian ditampilkan menggunakan directive `v-for`, sehingga setiap item dalam array otomatis dibuat menjadi satu card.

Struktur card menggunakan komponen Bootstrap dengan class `card` dan `card-body` untuk menjaga konsistensi tampilan. Gambar sertifikat dihubungkan menggunakan binding Vue `:src="cert.image"` sehingga sumber gambar mengikuti data yang telah didefinisikan.

Efek hover pada card diatur di dalam file `style.css` menggunakan properti `transform: translateY(-8px);` dan `transition` agar pergerakan terlihat halus. Warna background dan bayangan juga diatur dalam CSS untuk menjaga kesesuaian dengan tema utama website.

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
