# NB-Learning: Platform Try Out & Pembelajaran Inklusif (UI Prototype)

Repositori ini berisi prototipe antarmuka (Front-End) statis untuk platform **NB-Learning**, sebuah proyek berbasis web yang dirancang untuk memfasilitasi Try Out UTBK (CBT), forum diskusi, dan ekosistem pembelajaran *freemium*.

Proyek ini dikembangkan sebagai pemenuhan Tugas Akhir Semester (UAS) mata kuliah Workshop UI.

## 🚀 Teknologi yang Digunakan
* **HTML5:** Digunakan untuk membangun struktur semantik halaman web.
* **CSS3:** Digunakan untuk *styling*, tata letak (*Flexbox* dan *Grid*), serta penerapan variabel warna (*Design System*).
* **Desain Responsif:** Memanfaatkan *media queries* untuk memastikan tampilan tetap proporsional di berbagai perangkat.

## 📁 Struktur Halaman
Proyek ini mencakup beberapa antarmuka untuk berbagai ekosistem pengguna:
1. **Autentikasi & Landing:** `index.html`, `login.html`, `register.html`
2. **Siswa (Simulasi & Belajar):** `cbt.html` (Antarmuka Try Out), `score.html`, `leaderboard.html`
3. **Komunitas:** `forum.html`
4. **E-Commerce (Premium Store):** `katalog.html`, `detail-produk.html`, `keranjang.html`, `checkout.html`, `history.html`
5. **Dasbor Admin:** `admin.html` beserta antarmuka kelola data.

## ⚙️ Cara Menjalankan Proyek
Karena ini adalah prototipe Front-End statis, aplikasi ini tidak memerlukan instalasi *server lokal* (seperti XAMPP) atau *database*.
1. *Clone* atau unduh repositori ini.
2. Buka folder proyek di komputer Anda.
3. Klik ganda pada *file* `index.html`, atau seret *file* tersebut ke dalam peramban web (Google Chrome, Firefox, atau Safari).

---

## 🧪 Skenario Pengujian Sistem (UI/UX Testing)
Karena sistem ini berbasis prototipe statis (HTML & CSS), pengujian sistem difokuskan pada **Fungsionalitas Antarmuka, Responsivitas, dan Interaksi Visual**, bukan pada logika *backend*. Berikut adalah metrik pengujian yang telah dilakukan:

**1. Pengujian Responsivitas (Cross-Device Testing)**
* **Skenario:** Mengubah ukuran layar peramban ke resolusi *Mobile* (di bawah 768px) dan *Desktop*.
* **Hasil yang Diharapkan:** Elemen navigasi (*Navbar*) berubah menjadi *hamburger menu* atau tersusun rapi, struktur *grid* menyesuaikan (dari 3 kolom menjadi 1 kolom), dan tidak ada elemen yang meluber (*overflow*) ke luar layar.
* **Status:** Lulus (Teresolusi menggunakan *media query*).

**2. Pengujian Navigasi & Tautan Internal**
* **Skenario:** Mengklik seluruh tombol *Call to Action* (CTA), menu navigasi, dan *hyperlink* antar halaman statis.
* **Hasil yang Diharapkan:** Pengguna diarahkan ke *file* HTML yang tepat tanpa menemukan halaman *Error 404* (*broken link*).
* **Status:** Lulus.

**3. Pengujian Konsistensi Desain (Design System)**
* **Skenario:** Memvalidasi penggunaan warna, *border-radius*, *shadow*, dan tipografi di seluruh halaman (Siswa, Admin, dan E-commerce).
* **Hasil yang Diharapkan:** Seluruh halaman memiliki tampilan visual yang konsisten dan mengambil nilai gaya dari satu sumber *style* (seperti `admin-style.css`).
* **Status:** Lulus.

**4. Pengujian State & Interaksi Visual (Hover/Active)**
* **Skenario:** Mengarahkan kursor (*hover*) pada tombol, kartu produk, dan baris tabel (seperti di halaman *Leaderboard* atau tabel Admin).
* **Hasil yang Diharapkan:** Terjadi perubahan visual yang jelas (perubahan warna latar atau efek bayangan membesar) untuk memberikan *feedback* kepada pengguna bahwa elemen tersebut dapat diklik.
* **Status:** Lulus.