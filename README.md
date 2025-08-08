# 📁 Portofolio Pribadi

![Portofolio Web](https://res.cloudinary.com/dzsqaauqn/image/upload/v1754627248/Screenshot_2025-08-08_111921_tdddvc.jpg)

Portofolio pribadi adalah sebuah aplikasi web yang dibuat dengan **Python** menggunakan framework **Flask** dan database **MongoDB**. Proyek ini dirancang untuk menampilkan profil, proyek, dan artikel blog secara profesional.

---

## ✨ Fitur Utama

- **Halaman Beranda & Tentang Saya:** Pengenalan singkat tentang diri Anda dan ringkasan keahlian.
- **Daftar Proyek Dinamis:** Menampilkan daftar proyek yang diambil dari database, lengkap dengan fitur **pagination** untuk navigasi yang mudah.
- **Blog Dinamis:** Bagian blog untuk berbagi artikel, juga dilengkapi dengan **pagination**.
- **Formulir Kontak:** Pengunjung dapat mengirimkan pesan yang akan tersimpan ke database.
- **Halaman Pesan Admin:** Sebuah halaman sederhana untuk melihat daftar dan detail pesan yang masuk.
- **SEO On-Page Dinamis:** Implementasi SEO on-page, **sitemap.xml**, dan **robots.txt** untuk meningkatkan visibilitas di mesin pencari.
- **Meta Image & Favicon:** Dukungan untuk pratinjau media sosial (Open Graph) dan ikon situs.
- **Mode Gelap/Terang:** Pilihan tema visual yang dapat diubah oleh pengguna.
- **Responsif:** Desain yang dioptimalkan untuk berbagai ukuran perangkat, dari desktop hingga seluler.

---

## 🛠️ Teknologi yang Digunakan

|    Kategori   |                      Teknologi                       |
|---------------|------------------------------------------------------|
| **Backend**   | Python, Flask                                        |
| **Database**  | MongoDB, Cloudinary                                  |
| **Frontend**  | Jinja2 (HTML), Milligram.css, CSS Kustom, JavaScript |
| **Pustaka**   | PyMongo, python-dotenv                               |
| **Manajemen** | pip                                                  |
| **Deployment**| Vercel                                               |

---

## 🚀 Cara Menjalankan Proyek di Lokal

Ikuti langkah-langkah berikut untuk menjalankan proyek di komputer Anda.

### **1. Clone Repositori**
```bash
git clone https://github.com/IshikawaUta/portofolio_milligram_css
cd portofolio_milligram_css
```

### **2. Siapkan Virtual Environment**
```bash
python3 -m venv venv
source venv/bin/activate
```

### **3. Instal Ketergantungan**
Pastikan Anda telah membuat file `requirements.txt`.
```bash
pip install -r requirements.txt
```

### **4. Siapkan Database MongoDB**
Pastikan MongoDB sudah terinstal dan berjalan. Ubah baris kode koneksi di `app.py` jika Anda menggunakan host atau port yang berbeda.
```python
client = MongoClient('mongodb://localhost:27017/')
```

### **5. Jalankan Aplikasi**
```bash
flask run
```
Aplikasi Anda sekarang dapat diakses di `http://127.0.0.1:5000`.

---

## 🤝 Kontribusi

Jika Anda ingin berkontribusi, silakan fork repositori ini, buat branch baru, dan kirimkan **Pull Request**. Semua kontribusi sangat dihargai!
