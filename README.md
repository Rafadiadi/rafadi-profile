# Personal Portfolio Website - Muhammad Rafadi Kurniawan

Portfolio website profesional untuk freelance dan showcase project.

## 🚀 Fitur

- **Responsive Design** - Tampil sempurna di semua perangkat (desktop, tablet, mobile)
- **Modern UI/UX** - Design modern dengan gradient dan animasi smooth
- **Interactive Elements** - Animasi scroll, hover effects, dan typing effect
- **Contact Form** - Form kontak yang terintegrasi dengan email
- **Portfolio Showcase** - Section untuk menampilkan project-project Anda
- **Skills Display** - Visualisasi skills dengan progress bars
- **Social Media Links** - Link ke LinkedIn, GitHub, dan email

## 📁 Struktur File

```
Personal Web/
├── index.html          # File HTML utama
├── styles.css          # Styling CSS
├── script.js           # JavaScript functionality
├── images/             # Folder untuk gambar
│   └── rafadi.jpg      # Foto profil (tambahkan file ini)
└── README.md           # Dokumentasi
```

## 🎨 Kustomisasi

### 1. Tambahkan Foto Profil
- Letakkan foto Anda dengan nama `rafadi.jpg` di folder `images/`
- Ukuran rekomendasi: 500x500px atau 1:1 ratio
- Format: JPG, PNG, atau WebP

### 2. Update Informasi Portfolio
Edit file `index.html` di bagian portfolio untuk menambahkan project Anda:

```html
<div class="project-card">
    <div class="project-image">
        <img src="URL_GAMBAR_PROJECT" alt="Nama Project">
        ...
    </div>
    <div class="project-info">
        <h3>Nama Project</h3>
        <p>Deskripsi project</p>
        <div class="project-tags">
            <span class="tag">Teknologi 1</span>
            <span class="tag">Teknologi 2</span>
        </div>
    </div>
</div>
```

### 3. Customize Warna
Edit variabel CSS di `styles.css`:

```css
:root {
    --primary-color: #6366f1;      /* Warna utama */
    --secondary-color: #ec4899;    /* Warna sekunder */
    --accent-color: #f59e0b;       /* Warna aksen */
}
```

## 🌐 Cara Deploy

### Option 1: GitHub Pages (Gratis)
1. Buat repository baru di GitHub
2. Upload semua file ke repository
3. Pergi ke Settings > Pages
4. Pilih branch main/master
5. Website akan live di `https://username.github.io/repository-name`

### Option 2: Netlify (Gratis)
1. Pergi ke [Netlify](https://www.netlify.com/)
2. Drag & drop folder "Personal Web" ke Netlify
3. Website akan live dalam beberapa detik

### Option 3: Vercel (Gratis)
1. Install Vercel CLI: `npm i -g vercel`
2. Di folder project, jalankan: `vercel`
3. Ikuti instruksi di terminal

## 📱 Social Media Links

Pastikan untuk update link social media di file `index.html`:
- LinkedIn: https://www.linkedin.com/in/muhammad-rafadi-kurniawan-251067289
- GitHub: https://github.com/Rafadiadi
- Email: rafadiadi@gmail.com

## 🎯 Tips Optimasi

1. **Optimasi Gambar**
   - Compress foto sebelum upload
   - Gunakan format WebP untuk ukuran lebih kecil
   - Gunakan tools seperti TinyPNG atau Squoosh

2. **SEO**
   - Update meta tags di `<head>`
   - Tambahkan meta description
   - Gunakan alt text di semua gambar

3. **Performance**
   - Minimize CSS dan JavaScript saat production
   - Enable caching di hosting
   - Gunakan CDN untuk file besar

## 📞 Support

Jika ada pertanyaan atau issue:
- Email: rafadiadi@gmail.com
- LinkedIn: [Muhammad Rafadi Kurniawan](https://www.linkedin.com/in/muhammad-rafadi-kurniawan-251067289)

## 📄 License

Free to use for personal projects.

---

Made with ❤️ by Muhammad Rafadi Kurniawan
