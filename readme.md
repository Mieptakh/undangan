# 📋 Panduan Project Undangan Pernikahan Digital

## 🎯 Deskripsi Project
Project ini adalah undangan pernikahan digital interaktif untuk pasangan **Abi & Mufida** dengan tanggal pernikahan 30-31 Mei 2025. Undangan ini dibangun menggunakan HTML, CSS, JavaScript dan berbagai library modern untuk memberikan pengalaman yang menarik bagi tamu undangan.

## 🚀 Fitur Utama

### ✨ Fitur Interaktif
- **Welcome Screen**: Halaman sambutan dengan personalisasi nama tamu
- **Countdown Timer**: Penghitung mundur real-time menuju hari pernikahan
- **Love Story Timeline**: Timeline perjalanan cinta pasangan (2019-2025)
- **Interactive Gallery**: Carousel foto dengan navigasi smooth
- **Gift Section**: Informasi rekening untuk hadiah dengan fitur copy
- **Responsive Navigation**: Bottom navigation bar yang fixed

### 🎨 Fitur Visual
- **Smooth Animations**: Menggunakan AOS (Animate On Scroll)
- **Modern Design**: Gradient backgrounds dan glassmorphism effects
- **Custom Icons**: Font Awesome dan Lucide icons
- **Background Music**: Auto-play music dari YouTube
- **Floating Ornaments**: Dekorasi animasi di berbagai section

## 🛠 Teknologi yang Digunakan

### Framework & Library
- **Tailwind CSS** - Utility-first CSS framework
- **AOS (Animate On Scroll)** - Animation library
- **Glide.js** - Carousel/slider library
- **SweetAlert2** - Beautiful alert notifications
- **Font Awesome** - Icon library
- **Lucide** - Modern icon pack

### Font
- **Great Vibes** - Elegant script font
- **Open Sans** - Clean sans-serif font

### API & Services
- **YouTube IFrame API** - Background music player
- **Google Maps** - Location integration

## 📁 Struktur Project

```
undangan-pernikahan/
├── index.html              # File utama
├── foto/                   # Folder gambar
│   ├── WhatsApp Image 2025-05-27 at 08.56.03_7223fa05.jpg
│   ├── WhatsApp Image 2025-05-27 at 08.56.03_a266ac1a.jpg
│   ├── WhatsApp Image 2025-05-27 at 08.56.04_727355d4.jpg
│   └── 20250320_190104[1].png
└── README.md               # Dokumentasi
```

## 🎨 Color Palette

### Primary Colors (Hijau)
- **Primary 50**: `#f5f7f6` - Background terang
- **Primary 100**: `#e0e8e5` - Background sedang
- **Primary 400**: `#6f998e` - Accent
- **Primary 600**: `#42645c` - Button primary
- **Primary 700**: `#38514b` - Text primary
- **Primary 900**: `#2b3936` - Text dark

### Secondary Colors (Gold)
- **Secondary 400**: `#aa925e` - Gold accent
- **Secondary 500**: `#9b824d` - Gold primary
- **Secondary 600**: `#836a41` - Gold dark

## 📱 Sections Overview

### 1. Welcome Section
- **Background**: Hero image dengan overlay
- **Content**: Personalized greeting, couple names, CTA button
- **Features**: Fade-in animations, scroll prevention

### 2. Countdown Section
- **Content**: Wedding countdown timer, couple photo, Quranic verse
- **Features**: Real-time countdown, responsive grid layout

### 3. Couple Section
- **Content**: Bride and groom information, parents' names
- **Design**: Clean layout dengan typography hierarchy

### 4. Love Story Section
- **Content**: Timeline dari 2019-2025 dengan milestone penting
- **Design**: Vertical timeline dengan gradient line dan interactive cards

### 5. Schedule Section
- **Content**: Akad Nikah dan Resepsi details
- **Features**: Interactive cards dengan Google Maps integration

### 6. Gallery Section
- **Content**: Carousel foto pasangan
- **Features**: Glide.js carousel dengan navigation arrows dan bullets

### 7. Gift Section
- **Content**: Bank account information
- **Features**: Copy to clipboard functionality

### 8. Closing Section
- **Content**: Thank you message dan Instagram links
- **Design**: Floating hearts animation

## ⚙️ Instalasi & Setup

### Prerequisites
- Web browser modern (Chrome, Firefox, Safari, Edge)
- Web server (Apache, Nginx, atau live server untuk development)

### Langkah Instalasi

1. **Clone atau Download Project**
   ```bash
   git clone <repository-url>
   cd undangan-pernikahan
   ```

2. **Upload ke Hosting**
   - Upload semua file ke web hosting
   - Pastikan struktur folder tetap terjaga
   - Set index.html sebagai homepage

3. **Akses Undangan**
   ```
   https://domain-anda.com/
   ```

## 🔧 Kustomisasi

### Mengganti Informasi Pasangan

1. **Nama Pasangan**
   ```html
   <!-- Cari dan ganti di seluruh file -->
   <h1>Abi & Mufida</h1>
   <p>Mokhammad Abi Dullah Mukmin</p>
   <p>Mufidatul Alawiyah</p>
   ```

2. **Tanggal Pernikahan**
   ```javascript
   // Update di script countdown
   const weddingDate = new Date('May 30, 2025 19:00:00').getTime();
   ```

3. **Lokasi Acara**
   ```html
   <!-- Update alamat dan link Google Maps -->
   <p>Dsn Buaran RT 03 RW 09, Keboguyang, Jabon, Sidoarjo</p>
   <a href="https://maps.app.goo.gl/YwDCpXQZVbchUzBG6">
   ```

### Mengganti Foto

1. **Upload foto baru** ke folder `foto/`
2. **Update referensi** di HTML:
   ```html
   <img src="foto/nama-foto-baru.jpg" alt="Description">
   ```

### Menambah Tamu

1. **Edit guest list** di JavaScript:
   ```javascript
   const guestList = {
     "nama-parameter": "Nama Lengkap",
     // tambahkan tamu baru di sini
   };
   ```

2. **Akses dengan parameter**:
   ```
   https://domain-anda.com/?to=nama-parameter
   ```

### Mengganti Music

1. **Update YouTube video ID**:
   ```html
   <iframe src="https://www.youtube.com/embed/VIDEO-ID-BARU?...">
   ```

### Mengganti Rekening

```html
<!-- Update informasi bank -->
<h3>Bank BCA</h3>
<p>3151428001</p>
<p>a.n Mufidatul Alawiyah</p>
```

## 🎯 Fitur Personalisasi

### Guest List System
Undangan support personalisasi nama tamu melalui URL parameter:

```javascript
// Contoh penggunaan
https://domain-anda.com/?to=mita
// Akan menampilkan: "Kepada Yth. Mita"

https://domain-anda.com/?to=billy  
// Akan menampilkan: "Kepada Yth. Billy"
```

### Love Story Customization
Timeline dapat disesuaikan dengan mengedit section love-story:

```html
<!-- Tambah atau edit milestone -->
<div class="text-5xl font-bold text-primary-600">2026</div>
<div class="bg-white/80 backdrop-blur-lg shadow-md p-6 rounded-2xl">
  <h3>New Milestone</h3>
  <p>Description of the milestone</p>
</div>
```

## 📱 Responsive Design

Project ini fully responsive dengan breakpoints:
- **Mobile**: < 640px
- **Tablet**: 640px - 1024px  
- **Desktop**: > 1024px

### Mobile Optimizations
- Touch-friendly navigation
- Optimized image sizes
- Readable typography
- Smooth scrolling

## 🔍 SEO & Meta Tags

```html
<meta property="og:title" content="The Wedding of Abi & Mufida">
<meta property="og:description" content="Dengan penuh cinta kami mengundang Anda...">
<meta property="og:image" content="path-to-preview-image.jpg">
<meta property="og:url" content="https://domain-anda.com">
```

## ⚡ Performance Optimization

### Tips Optimasi
1. **Compress Images**: Gunakan tools seperti TinyPNG
2. **Minify CSS/JS**: Untuk production deployment
3. **Enable Gzip**: Di web server configuration
4. **CDN Usage**: Semua library sudah menggunakan CDN

### Loading Strategy
- Critical CSS inline
- Fonts preloaded
- Images lazy loaded
- Scripts deferred

## 🐛 Troubleshooting

### Common Issues

#### 1. Music Tidak Auto-play
**Solusi**: Modern browser memblokir auto-play. User harus interact dulu dengan page.

#### 2. Animation Tidak Smooth
**Solusi**: Pastikan AOS library loaded dengan benar:
```javascript
// Check di console
console.log(typeof AOS);
```

#### 3. Countdown Tidak Update
**Solusi**: Check timezone dan format tanggal:
```javascript
// Pastikan format tanggal benar
const weddingDate = new Date('May 30, 2025 19:00:00').getTime();
```

#### 4. Gambar Tidak Muncul
**Solusi**: Check path dan case-sensitive filenames:
```html
<!-- Pastikan path dan nama file exact match -->
<img src="foto/nama-file-exact.jpg">
```

## 🚀 Deployment

### Hosting Recommendations
1. **GitHub Pages** (Free)
2. **Netlify** (Free dengan custom domain)
3. **Vercel** (Free untuk personal projects)
4. **Shared Hosting** (cPanel based)

### Deployment Steps

#### GitHub Pages
1. Push ke GitHub repository
2. Enable GitHub Pages di settings
3. Akses via `username.github.io/repository-name`

#### Netlify
1. Connect GitHub repository
2. Auto-deploy on push
3. Custom domain available

## 📊 Analytics & Monitoring

### Recommended Tools
- **Google Analytics** - Traffic monitoring
- **Google Search Console** - SEO monitoring
- **PageSpeed Insights** - Performance testing

### Implementation
```html
<!-- Add before closing </head> -->
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

## 🔐 Security Best Practices

1. **No Sensitive Data**: Jangan hardcode data sensitif
2. **HTTPS Only**: Gunakan SSL certificate
3. **Input Validation**: Sanitize user inputs
4. **Regular Updates**: Update dependencies secara berkala

## 🎁 Additional Features Ideas

### Possible Enhancements
- **RSVP System** dengan database
- **Live Wedding Stream** integration
- **Guest Book** dengan comments
- **Wedding Registry** integration
- **Push Notifications** untuk reminder
- **QR Code Generator** untuk easy sharing

## 📝 License & Credits

### Credits
- **Design**: Custom design untuk Abi & Mufida
- **Development**: @mh.teams
- **Icons**: Font Awesome & Lucide
- **Animations**: AOS Library
- **Carousel**: Glide.js

### Usage Rights
Project ini dibuat khusus untuk pernikahan Abi & Mufida. Untuk penggunaan pada acara lain, silakan modifikasi sesuai kebutuhan dengan tetap memberikan credit yang sesuai.

---

## 🤝 Support & Contact

Untuk pertanyaan atau bantuan lebih lanjut, silakan hubungi:
- **Instagram**: [@mh.teams](https://instagram.com/mh.teams)
- **Developer**: MH Teams

---

*Semoga pernikahan Abi & Mufida bahagia selalu! 💕*