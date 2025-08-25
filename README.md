# 🚗 Araç Filo Yönetim Sistemi

**Versiyon:** v22.07.24.01  
**Geliştirici:** Ertuğrul Kamil ŞAHİN  
**GitHub:** [https://github.com/ertugrul-yazilim/arac.filo](https://github.com/ertugrul-yazilim/arac.filo)

---

## 📋 İçindekiler

- [Özellikler](#-özellikler)
- [Kurulum](#-kurulum)
- [Kullanım](#-kullanım)
- [Güncelleme](#-güncelleme)
- [Teknik Detaylar](#-teknik-detaylar)
- [Sorun Giderme](#-sorun-giderme)
- [Katkıda Bulunma](#-katkıda-bulunma)
- [Lisans](#-lisans)

---

## ✨ Özellikler

### 🚗 Araç Yönetimi
- **Araç Kayıt**: Plaka, marka, model, yıl bilgileri
- **Araç Takibi**: KM, yakıt tüketimi, durum bilgileri
- **Fotoğraf Desteği**: Her araç için fotoğraf ekleme
- **Detaylı Bilgiler**: Motor, şanzıman, renk, vb.

### 🔧 Bakım Yönetimi
- **Bakım Kayıtları**: Tarih, KM, servis bilgileri
- **Maliyet Takibi**: Bakım tutarları ve detayları
- **Bakım Geçmişi**: Araç bazında bakım geçmişi
- **Otomatik Hatırlatma**: Bakım zamanı yaklaşan araçlar

### 👨‍💼 Sürücü Yönetimi
- **Sürücü Kayıtları**: Kişisel bilgiler, ehliyet detayları
- **Zimmet Takibi**: Hangi araç kimde
- **Sürücü Geçmişi**: Araç kullanım geçmişi

### 📊 Raporlama
- **Excel Export**: Tüm verileri Excel formatında dışa aktırma
- **PDF Raporları**: Detaylı PDF raporları
- **İstatistikler**: Filo performans analizi
- **Grafikler**: Görsel veri analizi

### 🔄 Otomatik Güncelleme
- **GitHub Entegrasyonu**: Otomatik versiyon kontrolü
- **Güncelleme Bildirimi**: Yeni sürüm uyarıları
- **Kolay İndirme**: GitHub üzerinden güncelleme

### 💾 Veri Yönetimi
- **Otomatik Yedekleme**: Veri güvenliği
- **Excel Entegrasyonu**: Mevcut Excel dosyalarıyla uyum
- **Veri İçe Aktarma**: Toplu veri yükleme

---

## 🛠️ Kurulum

### Gereksinimler
- **Python 3.8+**
- **Windows 10/11** (Test edildi)
- **İnternet Bağlantısı** (Güncelleme kontrolü için)

### Adım 1: Python Kurulumu
```bash
# Python'u https://python.org adresinden indirin
# Kurulum sırasında "Add Python to PATH" seçeneğini işaretleyin
```

### Adım 2: Proje İndirme
```bash
# GitHub'dan projeyi indirin
git clone https://github.com/ertugrul-yazilim/arac.filo.git
cd arac.filo
```

### Adım 3: Bağımlılıkları Yükleme
```bash
# Gerekli kütüphaneleri yükleyin
pip install -r requirements.txt
```

### Adım 4: Programı Çalıştırma
```bash
# Ana programı başlatın
python arac1.py
```

---

## 🚀 Kullanım

### İlk Çalıştırma
1. Program başladığında otomatik güncelleme kontrolü yapılır
2. Yeni sürüm varsa indirme seçeneği sunulur
3. Ana ekranda dashboard görüntülenir

### Ana Menü
- **🏠 Dashboard**: Genel bakış ve istatistikler
- **🚗 Araçlar**: Araç yönetimi
- **🔧 Bakımlar**: Bakım kayıtları
- **👨‍💼 Sürücüler**: Sürücü yönetimi
- **📊 Raporlar**: Raporlama araçları
- **⚙️ Ayarlar**: Sistem ayarları

### Klavye Kısayolları
- **Ctrl+N**: Yeni kayıt
- **Ctrl+S**: Kaydet
- **Ctrl+E**: Düzenle
- **Delete**: Sil
- **F5**: Yenile
- **Ctrl+F**: Ara
- **Ctrl+P**: Yazdır

---

## 🔄 Güncelleme

### Otomatik Güncelleme
- Program her başladığında GitHub'dan versiyon kontrolü yapar
- Yeni sürüm varsa kullanıcıya bildirir
- İndirme seçeneği sunar

### Manuel Güncelleme
1. **Ayarlar** → **Güncelleme Ayarları**
2. **"Güncelleme Kontrol Et"** butonuna tıklayın
3. Yeni sürüm varsa indirme linki görüntülenir

### Güncelleme Geçmişi
- **v22.07.24.01**: İlk kararlı sürüm
- **v22.07.24.02**: GitHub entegrasyonu eklendi

---

## 🔧 Teknik Detaylar

### Kullanılan Teknolojiler
- **Python 3.8+**: Ana programlama dili
- **PyQt5**: GUI framework
- **Pandas**: Veri işleme
- **OpenPyXL**: Excel dosya işlemleri
- **ReportLab**: PDF rapor oluşturma
- **Requests**: HTTP istekleri (GitHub API)

### Dosya Yapısı
```
arac/
├── arac1.py                    # Ana program
├── requirements.txt            # Bağımlılıklar
├── araba_icon.png             # Program ikonu
├── README.md                  # Bu dosya
└── veri/                      # Veri klasörü
    ├── araclar.xlsx           # Araç verileri
    ├── bakimlar.xlsx          # Bakım verileri
    ├── suruculer.xlsx         # Sürücü verileri
    └── ...                    # Diğer veri dosyaları
```

### Veri Formatları
- **Excel (.xlsx)**: Ana veri formatı
- **PDF**: Rapor formatı
- **JSON**: Konfigürasyon dosyaları

---

## 🐛 Sorun Giderme

### Yaygın Sorunlar

#### Program Başlamıyor
```bash
# Python versiyonunu kontrol edin
python --version

# Bağımlılıkları yeniden yükleyin
pip install -r requirements.txt --force-reinstall
```

#### Excel Dosyaları Açılmıyor
- Excel dosyalarının kilitli olmadığından emin olun
- Dosya izinlerini kontrol edin
- Antivirüs programını geçici olarak devre dışı bırakın

#### Güncelleme Kontrolü Çalışmıyor
- İnternet bağlantınızı kontrol edin
- Firewall ayarlarını kontrol edin
- GitHub erişimini test edin

#### Veri Kaybı
- `veri/` klasöründeki yedek dosyaları kontrol edin
- Excel dosyalarının yedeğini alın
- Program loglarını inceleyin

### Log Dosyaları
Program logları şu konumda saklanır:
```
%APPDATA%/AracFilo/logs/
```

### Hata Raporlama
Hata durumunda:
1. Log dosyalarını kontrol edin
2. Hata mesajını not edin
3. GitHub Issues'da raporlayın

---

## 🤝 Katkıda Bulunma

### Geliştirme Ortamı
```bash
# Projeyi fork edin
git clone https://github.com/your-username/arac.filo.git
cd arac.filo

# Geliştirme bağımlılıklarını yükleyin
pip install -r requirements-dev.txt

# Test edin
python -m pytest tests/
```

### Kod Standartları
- **PEP 8**: Python kod standartları
- **Type Hints**: Tip belirteçleri kullanın
- **Docstrings**: Fonksiyon dokümantasyonu
- **Türkçe**: Yorumlar ve değişken isimleri Türkçe

### Pull Request Süreci
1. Feature branch oluşturun
2. Değişikliklerinizi yapın
3. Testleri çalıştırın
4. Pull request gönderin

---

## 📄 Lisans

Bu proje **MIT Lisansı** altında lisanslanmıştır.

```
MIT License

Copyright (c) 2024 Ertuğrul Yazılım

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 📞 İletişim

- **GitHub**: [https://github.com/ertugrul-yazilim/arac.filo](https://github.com/ertugrul-yazilim/arac.filo)
- **E-posta**: [ertugrul.yazilim@gmail.com](mailto:ertugrul.yazilim@gmail.com)
---

## 🙏 Teşekkürler

Bu projeyi geliştirmemizde yardımcı olan herkese teşekkürler!

- **PyQt5** geliştiricileri
- **Pandas** ekibi
- **GitHub** platformu
- **Açık kaynak topluluğu**

---

**Son Güncelleme:** 25.08.2025  
**Versiyon:** v22.07.24.01
