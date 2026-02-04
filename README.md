# Kozmik Nötron Dedektörü Projesi Web Sitesi

Modern, Türkçe statik web sitesi - TÜBİTAK 1001 Projesi (Proje No: 123F253)

**Proje Başlığı:** Kozmik Nötron Tespiti için Sintilasyon Tozları ve Optik Ortamların Potansiyelinin Araştırılması

**Proje Yürütücüsü:** Prof. Dr. Taylan Yetkin  
**Kurum:** İstinye Üniversitesi

---

## 📋 İçindekiler

- [Proje Hakkında](#proje-hakkında)
- [Özellikler](#özellikler)
- [Teknolojiler](#teknolojiler)
- [Kurulum ve Yerel Geliştirme](#kurulum-ve-yerel-geliştirme)
- [GitHub'a Yükleme](#githuba-yükleme)
- [Cloudflare Pages ile Yayınlama](#cloudflare-pages-ile-yayınlama)
- [Proje Yapısı](#proje-yapısı)

---

## 🔬 Proje Hakkında

Bu web sitesi, kozmik nötron dedektörü geliştirme projesinin araştırma hedeflerini, teknolojisini ve bilimsel arka planını tanıtmak için oluşturulmuştur. Proje, gazlı dedektörlere alternatif olarak toz sintilatörleri ve optik ortamlar kullanarak yüksek verimli, güvenli nötron dedektörleri geliştirmeyi amaçlamaktadır.

---

## ✨ Özellikler

- 🌌 **Modern Kozmik Tema:** Karanlık arka plan, canlı gradyanlar ve yumuş ak animasyonlar
- 📱 **Tam Responsive:** Mobil, tablet ve masaüstü cihazlarda mükemmel görünüm
- 🎯 **Tek Sayfa Tasarım:** Akıcı gezinme ve kaydırma deneyimi
- ⚡ **Performans Optimize:** Hızlı yükleme ve pürüzsüz animasyonlar
- 🎨 **Görsel Hikaye Anlatımı:** İnfografikler, ikonlar ve kartlarla bilgi sunumu
- 🌍 **SEO Optimize:** Arama motorları için optimize edilmiş meta etiketler
- ♿ **Erişilebilirlik:** ARIA etiketleri ve klavye navigasyonu desteği

---

## 🛠️ Teknolojiler

Bu proje **saf HTML, CSS ve JavaScript** kullanılarak geliştirilmiştir:

- **HTML5** - Semantik yapı
- **CSS3** - Modern tasarım sistemi (CSS değişkenleri, Flexbox, Grid)
- **Vanilla JavaScript** - İnteraktif özellikler (framework yok)
- **Google Fonts (Inter)** - Modern tipografi

---

## 💻 Kurulum ve Yerel Geliştirme

### Ön Gereksinimler

Sadece bir web tarayıcısı gereklidir. Statik bir site olduğu için ek kurulum gerekmez.

### Adım 1: Yerel Sunucu Başlatma

Basit bir HTTP sunucusu başlatmak için aşağıdaki yöntemlerden birini kullanın:

**Python 3 kullanarak:**
```bash
cd /Users/tyetkin/Work/neutron_detectors_web/kozmikparcaciklar
python3 -m http.server 8000
```

**Python 2 kullanarak:**
```bash
python -m SimpleHTTPServer 8000
```

**Node.js live-server kullanarak:**
```bash
npx live-server
```

### Adım 2: Tarayıcıda Açma

Sunucu başlatıldıktan sonra tarayıcınızda şu adresi açın:
```
http://localhost:8000
```

---

## 📤 GitHub'a Yükleme

### Adım 1: Git Deposunu Kontrol Etme

Repository zaten bağlı olmalı. Kontrol için:

```bash
cd /Users/tyetkin/Work/neutron_detectors_web/kozmikparcaciklar
git status
```

### Adım 2: Dosyaları Ekleme ve Commit

```bash
# Tüm dosyaları staging area'ya ekle
git add .

# Commit oluştur
git commit -m "İlk commit: Kozmik Nötron Dedektörü web sitesi"
```

### Adım 3: GitHub'a Push

```bash
# Main branch'e push et
git push origin main
```

> **Not:** Eğer branch adı `master` ise:
> ```bash
> git push origin master
> ```

### Adım 4: GitHub'da Kontrol

1. GitHub repository'nizi açın: `https://github.com/tyetkin/kozmikparcaciklar`
2. Tüm dosyaların yüklendiğini doğrulayın

---

## ☁️ Cloudflare Pages ile Yayınlama

### Adım 1: Cloudflare Pages'e Giriş

1. [Cloudflare Dashboard](https://dash.cloudflare.com/)'a gidin
2. Sol menüden **Pages** seçin
3. **Create a project** butonuna tıklayın

### Adım 2: GitHub Repository Bağlama

1. **Connect to Git** seçin
2. **GitHub** seçeneğini seçin
3. GitHub hesabınıza giriş yapın (gerekirse)
4. `tyetkin/kozmikparcaciklar` repository'sini seçin
5. **Begin setup** butonuna tıklayın

### Adım 3: Build Ayarları

Aşağıdaki ayarları yapın:

- **Project name:** `kozmikparcaciklar` (veya istediğiniz isim)
- **Production branch:** `main` (veya `master`)
- **Framework preset:** `None` (statik site)
- **Build command:** *(Boş bırakın)*
- **Build output directory:** `/` (kök dizin)

### Adım 4: Deployment

1. **Save and Deploy** butonuna tıklayın
2. Build sürecini izleyin (genellikle 1-2 dakika sürer)
3. Deployment tamamlandığında yeşil "Success" mesajı göreceksiniz

### Adım 5: Site URL'si

Deployment tamamlandıktan sonra:
- Cloudflare otomatik olarak bir URL oluşturur: `https://kozmikparcaciklar.pages.dev`
- Bu URL üzerinden sitenizi test edebilirsiniz

### Adım 6 (Opsiyonel): Custom Domain

Kendi domain adınızı kullanmak isterseniz:

1. Cloudflare Pages projenizde **Custom domains** sekmesine gidin
2. **Set up a custom domain** butonuna tıklayın
3. Domain adınızı girin ve talimatları izleyin

---

## 🚀 Güncelleme Yapma

Site güncellemek için:

```bash
# Değişiklikleri yap (HTML, CSS veya JS dosyalarını düzenle)

# Git'e ekle
git add .

# Commit oluştur
git commit -m "Güncelleme açıklaması"

# GitHub'a push et
git push origin main
```

> **Otomatik Deployment:** Cloudflare Pages, `main` branch'e her push yaptığınızda otomatik olarak siteyi güncelleyecektir.

---

## 📁 Proje Yapısı

```
kozmikparcaciklar/
├── index.html          # Ana HTML dosyası
├── styles.css          # CSS stilleri
├── script.js           # JavaScript kodu
├── README.md           # Bu dosya
└── .gitignore          # Git ignore dosyası
```

### Dosya Açıklamaları

- **index.html** - Web sitesinin tüm içeriğini ve yapısını içerir
- **styles.css** - Modern kozmik tema, responsive tasarım ve animasyonlar
- **script.js** - Smooth scrolling, mobil menü, animasyonlar ve interaktif özellikler
- **README.md** - Proje dokümantasyonu ve deployment kılavuzu
- **.gitignore** - Git tarafından takip edilmeyecek dosyalar

---

## 🔧 Özelleştirme

### Renkler

CSS değişkenlerini düzenleyerek renk temasını değiştirebilirsiniz (`styles.css` dosyasının başında):

```css
:root {
    --color-primary: #6366f1;        /* Ana renk */
    --color-secondary: #8b5cf6;      /* İkincil renk */
    --color-accent: #ec4899;         /* Vurgu rengi */
}
```

### İçerik

Tüm içerik `index.html` dosyasında bulunur. İlgili bölümleri düzenleyerek güncelleyebilirsiniz.

### Animasyonlar

Animasyonları `styles.css` dosyasında `@keyframes` kurallarını düzenleyerek özelleştirebilirsiniz.

---

## 📞 İletişim

**Proje Yürütücüsü:** Prof. Dr. Taylan Yetkin  
**E-posta:** tyetkin@istinye.edu.tr  
**Kurum:** İstinye Üniversitesi

**Proje No:** TÜBİTAK 1001 - 123F253

---

## 📄 Lisans

© 2026 İstinye Üniversitesi. Tüm hakları saklıdır.

---

## 🙏 Teşekkürler

Bu proje TÜBİTAK 1001 - Bilimsel ve Teknolojik Araştırma Projeleri Destekleme Programı kapsamında desteklenmektedir.
