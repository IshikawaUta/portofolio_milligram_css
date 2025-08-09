# 📁 Portofolio Pribadi (Milligram CSS)

![Portofolio Web](https://res.cloudinary.com/dzsqaauqn/image/upload/v1754627248/static/assets/img/Screenshot_2022-10-06_144212_qeyf6j.png)

## Deskripsi Proyek

Ini adalah proyek portofolio pribadi yang dibangun menggunakan **Python** dan framework web **Flask**. Tujuan utama proyek ini adalah untuk menampilkan pekerjaan dan kemampuan Anda sebagai pengembang web *full-stack*, dengan fitur dinamis seperti daftar proyek, blog, dan formulir kontak. Proyek ini dirancang agar mudah dikelola dan siap untuk di-*deploy* ke platform modern.

### Fitur Unggulan:
* **Sistem Manajemen Konten (CMS) Sederhana**: Dasbor admin yang dilindungi kata sandi memungkinkan Anda untuk menambah, mengedit, dan menghapus proyek serta postingan blog.
* **Database NoSQL**: Menggunakan MongoDB Atlas untuk penyimpanan data proyek, blog, kontak, dan ulasan.
* **Penyimpanan Media Cloud**: Mengintegrasikan Cloudinary untuk menyimpan dan mengelola gambar, memastikan performa situs yang cepat.
* **Optimasi SEO**: Dilengkapi dengan `sitemap.xml` dan `robots.txt` untuk membantu *crawler* mesin pencari mengindeks situs Anda dengan lebih efektif.
* **Pengalaman Pengguna (UX) yang Baik**: Mendukung mode gelap/terang, desain responsif, dan tombol "Scroll Up" untuk navigasi yang nyaman.
* **Otomatisasi Email**: Menggunakan Flask-Mail untuk mengirim email notifikasi secara otomatis dari formulir kontak.

---

## Tumpukan Teknologi
* **Bahasa Pemrograman**: Python
* **Framework Backend**: Flask
* **Templating Engine**: Jinja2
* **Styling**: Milligram.css (kerangka kerja CSS minimalis), CSS kustom
* **Interaksi Frontend**: JavaScript kustom
* **Database**: MongoDB (melalui PyMongo)
* **Penyimpanan Media**: Cloudinary
* **Lainnya**: `python-dotenv` untuk manajemen variabel lingkungan, `Flask-Login`, `Flask-Mail`

---

## Struktur Direktori
```
📦 your_project
┣ 📂 templates/
┃ ┣ 📜 admin_blog_dashboard.html
┃ ┣ 📜 admin_dashboard.html
┃ ┣ 📜 admin_login.html
┃ ┣ 📜 admin_reviews.html
┃ ┣ 📜 add_blog.html
┃ ┣ 📜 add_project.html
┃ ┣ 📜 add_review.html
┃ ┣ 📜 edit_blog.html
┃ ┣ 📜 edit_project.html
┃ ┣ 📜 about.html
┃ ┣ 📜 base.html
┃ ┣ 📜 blog_post.html
┃ ┣ 📜 blog.html
┃ ┣ 📜 contact.html
┃ ┣ 📜 index.html
┃ ┣ 📜 message_detail.html
┃ ┣ 📜 messages.html
┃ ┣ 📜 projects.html
┃ ┣ 📜 reviews.html
┃ ┣ 📜 services.html
┃ ┣ 📜 robots.txt
┃ ┗ 📜 sitemap.xml
┣ 📂 static/
┃ ┣ 📂 css/
┃ ┃ ┣ 📜 custom.css
┃ ┃ ┗ 📜 milligram.css
┃ ┗ 📂 js/
┃   ┗ 📜 custom.js
┣ 📜 .env
┣ 📜 app.py
┣ 📜 README.md
┣ 📜 requirements.txt
┗ 📜 vercel.json

```

---

## Persiapan dan Instalasi

### 1. Kloning Repositori
```bash
git clone https://github.com/IshikawaUta/portofolio_milligram_css
cd portofolio_milligram_css
```

### 2. Buat Virtual Environment
Pastikan Anda berada di direktori proyek, lalu jalankan perintah berikut:
```bash
python -m venv venv
```
Untuk mengaktifkan virtual environment:

* **Windows**: `venv\Scripts\activate`
* **macOS/Linux**: `source venv/bin/activate`

### 3. Instal Ketergantungan
Instal semua pustaka yang diperlukan dari file `requirements.txt`:
```bash
pip install -r requirements.txt
```

### 4. Konfigurasi Variabel Lingkungan
Buat file `.env` di direktori utama proyek dan tambahkan konfigurasi berikut:
```
MONGO_URI=<URI_MONGODB_ATLAS_ANDA>
FLASK_MAIL_USERNAME=<EMAIL_PENGIRIM_ANDA>
FLASK_MAIL_PASSWORD=<KATA_SANDI_EMAIL_ANDA>
CLOUDINARY_CLOUD_NAME=<NAMA_CLOUD_CLOUDINARY>
CLOUDINARY_API_KEY=<API_KEY_CLOUDINARY>
CLOUDINARY_API_SECRET=<API_SECRET_CLOUDINARY>
ADMIN_USERNAME=admin
ADMIN_PASSWORD_HASH=<HASH_KATA_SANDI_ADMIN>
```
**Catatan**: Anda dapat membuat hash kata sandi menggunakan Python atau alat online lainnya.

### 5. Menjalankan Proyek Secara Lokal
Setelah semua persiapan selesai, Anda dapat menjalankan aplikasi Flask:
```bash
flask run
```
Aplikasi akan berjalan di `http://127.0.0.1:5000`.

---

## Deployment ke Vercel
Proyek ini telah dikonfigurasi untuk di-*deploy* dengan mudah menggunakan Vercel. File `vercel.json` sudah disiapkan untuk mengarahkan semua rute ke `app.py`. Cukup sambungkan repositori Git Anda ke Vercel, dan Vercel akan otomatis mendeteksi konfigurasi dan melakukan deployment.
