<div align="center">

# 🏛️ Vue.js + MySQL Kütüphane Paneli

**BMU1208 Web Tabanlı Programlama — Final Projesi**

![Vue](https://img.shields.io/badge/Vue.js-3.x-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white)
![Node](https://img.shields.io/badge/Node.js-18.x-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-3.x-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

> *Vue 3 + MySQL ile kampus kutuphaneleri icin modern odunc/iade paneli*

**Hazirlayan:** Nazar Eylul Sayinda | **Ogrenci No:** 24080410213  
**Universite:** Bitlis Eren Universitesi — Muhendislik-Mimarlik Fakultesi  
**Bolum:** Bilgisayar Muhendisligi

</div>

---

## 📸 Ekran Goruntuleri

| Dashboard | Kitaplar | Odunc Takibi |
|:---------:|:--------:|:------------:|
| ![Dashboard](docs/screenshots/dashboard.png) | ![Kitaplar](docs/screenshots/books.png) | ![Odunc](docs/screenshots/borrows.png) |

| Giris Ekrani | Istatistikler | Kullanicılar |
|:------------:|:-------------:|:------------:|
| ![Login](docs/screenshots/login.png) | ![Stats](docs/screenshots/stats.png) | ![Users](docs/screenshots/users.png) |

---

## ✨ Ozellikler

### 🎨 Admin Paneli
- 📊 **Dashboard** — Chart.js ile interaktif istatistik grafikleri
- 📚 **Kitap Yonetimi** — Ekleme, duzenleme, silme, kategori filtreleme
- 👥 **Kullanici Yonetimi** — Rol tabanli erisim (Admin / Uye)
- 📅 **Takvim** — Odunc/iade tarihleri gorsel takvimde
- ⚠️ **Gecikme Takibi** — Suresi gecmis iadeleri otomatik listele
- 🔔 **Bildirim Sistemi** — Gercek zamanli bildirimler

### 👤 Uye Paneli
- 📖 **Kitap Katalogu** — Galeri ve liste gorunumu, arama & filtre
- 📋 **Odunclerim** — Aktif odunc listesi ve gecmis
- 🌙 **Karanlik Mod** — 6 farkli tema rengi secenegi
- 👤 **Profil & Ayarlar** — Kisisel bilgi guncelleme

---

## 🛠️ Teknoloji Yigini

| Katman | Teknoloji |
|--------|-----------|
| **Frontend** | Vue 3 (Composition API), Vue Router, Tailwind CSS |
| **Backend** | Node.js, Express.js, REST API |
| **Veritabani** | MySQL 8.0 |
| **Kimlik Dogrulama** | JWT + Bcrypt |
| **Grafikler** | Chart.js |
| **Container** | Docker + Docker Compose |

---

## 🚀 Kurulum

### Gereksinimler
- Node.js 18+
- MySQL 8.0+
- npm

### 1. Veritabanini Hazirla
```sql
CREATE DATABASE library_db;
-- database/schema.sql dosyasini import et
```

### 2. Backend
```bash
cd backend
npm install
cp .env.example .env   # .env dosyasini duzenle
npm start              # http://localhost:3000
```

### 3. Frontend
```bash
cd frontend
npm install
npm run dev            # http://localhost:5173
```

### Docker ile Tek Komut
```bash
docker-compose up --build
```

---

## 🏗️ Proje Yapisi

```
repo/
├── backend/
│   ├── routes/        # API endpoint'leri
│   ├── middleware/    # JWT kimlik dogrulama
│   ├── config/        # Veritabani baglantisi
│   └── server.js      # Ana sunucu
├── frontend/
│   └── src/
│       ├── views/     # Sayfa bilesenler (Admin + Uye)
│       ├── components/ # Sidebar, Topbar vb.
│       ├── router/    # Vue Router
│       └── state/     # Global state yonetimi
├── database/
│   └── schema.sql     # Tam veritabani semasi
└── docs/
    ├── diagrams/      # C4 mimari diyagramlari
    └── screenshots/   # Ekran goruntuleri
```

---

## 📦 Indirme

Projenin tam zip paketini [Releases](https://github.com/nazareylulsayinda/vue-mysql-kutuphane-paneli/releases/latest) bolumunden indirebilirsiniz.

---

## 📄 Lisans

Bu proje [MIT Lisansi](LICENSE) altinda lisanslanmistir.

---

<div align="center">

**Gelistiren:** [Nazar Eylul Sayinda](https://github.com/nazareylulsayinda) 🚀

*Bitlis Eren Universitesi — Bilgisayar Muhendisligi — 2025/2026*

</div>