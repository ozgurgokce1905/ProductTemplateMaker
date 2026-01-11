# ProductTemplateMaker

🎨 **E-ticaret ve sosyal medya için ürün görseli şablonu tasarlama uygulaması**

![.NET Framework](https://img.shields.io/badge/.NET%20Framework-4.7.2+-blue)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)

ProductTemplateMaker, e-ticaret platformları (Trendyol, Hepsiburada vb.) ve sosyal medya (Instagram, Facebook) için profesyonel ürün görselleri oluşturmanızı sağlayan bir Windows masaüstü uygulamasıdır.

## ✨ Özellikler

### 📐 Hazır Format Desteği
- **Instagram Hikaye** (1080x1920)
- **Instagram Kare** (1080x1080)
- **Instagram 4:5** (1080x1350)
- **Facebook Hikaye** (1080x1920)
- **Facebook Kare** (1080x1080)
- **Trendyol** (1200x1800)
- **Özel Boyut** - İstediğiniz ölçüleri girin

### 🖼️ Görsel İşlemleri
- Arka plan görseli ekleme ve düzenleme
- Ürün görseli ekleme (tekli veya çoklu)
- PNG destekli şeffaf görsel desteği
- Görsel döndürme ve ölçekleme
- Opaklık (saydamlık) ayarı

### 📝 Metin ve Rozet Araçları
- Özelleştirilebilir metin kutuları
- Çeşitli rozet şekilleri:
  - Dörtgen
  - Yuvarlatılmış köşeli
  - Elips / Daire
  - Üçgen
  - Yıldız (5 köşeli)
  - Altıgen
  - Beşgen
  - Ok şekli
- PNG rozet desteği (kendi görsellerinizi kullanın)
- Font, renk ve hizalama ayarları
- Şeffaf veya renkli arka plan seçeneği

### 🎯 Dikey Bar (Yan Şerit)
- Ürün bilgisi için dikey metin alanı
- Özelleştirilebilir bar ve yazı rengi
- Alpha (saydamlık) kontrolü

### 🔧 Düzenleme Araçları
- Sürükle & bırak ile konumlandırma
- Köşelerden boyutlandırma
- Döndürme desteği
- Z-sıralaması (öne getir / arkaya gönder)
- Oran koruyarak boyutlandırma
- Undo (Geri Al) desteği - Ctrl+Z

### 🔍 Görünüm Kontrolleri
- Zoom (yakınlaştırma/uzaklaştırma): %25 - %400
- Otomatik sığdırma modu
- Scroll ile gezinme

### 💾 Dışa Aktarma
- Yüksek kaliteli PNG export
- Tasarım boyutunda (örn: 1200x1800) temiz çıktı

## 📸 Ekran Görüntüleri

*Ekran görüntüleri eklenecek*

## 🚀 Kurulum

### Gereksinimler
- Windows 10/11
- .NET Framework 4.7.2 veya üzeri
- Visual Studio 2019/2022 (geliştirme için)

### Çalıştırma

1. Projeyi klonlayın:
```bash
git clone https://github.com/kullaniciadi/ProductTemplateMaker.git
```

2. Visual Studio ile `ProductTemplateMaker.sln` dosyasını açın

3. Projeyi derleyin (Build > Build Solution veya Ctrl+Shift+B)

4. Çalıştırın (F5 veya Debug > Start Debugging)

### Release Versiyonu
Derlenmiş hazır uygulamayı [Releases](https://github.com/kullaniciadi/ProductTemplateMaker/releases) sayfasından indirebilirsiniz.

## 📖 Kullanım

### Hızlı Başlangıç

1. **Format Seçin**: Sağ panelden hedef platformunuza uygun formatı seçin
2. **Arka Plan Ekleyin**: "Fon Seç" butonu ile arka plan görseli yükleyin
3. **Ürün Ekleyin**: "Ürün Seç" veya "Ürün +" butonları ile ürün görsellerinizi ekleyin
4. **Metin/Rozet Ekleyin**: Fiyat, indirim oranı veya kampanya bilgisi için metin ve rozetler ekleyin
5. **Düzenleyin**: Nesneleri sürükleyerek konumlandırın, köşelerden boyutlandırın
6. **Dışa Aktarın**: "Export" butonu ile PNG olarak kaydedin

### Klavye Kısayolları

| Kısayol | İşlev |
|---------|-------|
| `Ctrl + Z` | Geri Al (Undo) |
| `Delete` | Seçili nesneyi sil |
| `Mouse Scroll` | Zoom (Ctrl basılıyken) |

### İpuçları

- **Oran Koruma**: "Oran" kutusunu işaretleyerek boyutlandırırken oranı koruyun
- **Hassas Konumlandırma**: En/Boy değerlerini numerik kutulardan manuel girin
- **Şeffaf Rozetler**: PNG rozet özelliğini kullanarak kendi tasarımlarınızı ekleyin

## 🏗️ Proje Yapısı

```
ProductTemplateMaker/
├── ProductTemplateMaker.sln      # Solution dosyası
└── ProductTemplateMaker/
    ├── ProductTemplateMaker.csproj
    ├── Form1.cs                  # Ana form ve tüm mantık
    ├── Program.cs                # Uygulama giriş noktası
    └── Properties/
        └── AssemblyInfo.cs
```

### Temel Sınıflar

| Sınıf | Açıklama |
|-------|----------|
| `Form1` | Ana uygulama formu ve UI kontrolü |
| `CanvasControl` | Tasarım canvas'ı - çizim ve etkileşim |
| `Element` | Tüm canvas nesneleri için temel sınıf |
| `TextElement` | Metin ve rozet nesnesi |
| `ImageElement` | Ürün görseli nesnesi |
| `ImageTextElement` | PNG rozet + metin nesnesi |
| `BarElement` | Dikey bar (yan şerit) nesnesi |

## 🤝 Katkıda Bulunma

Katkılarınızı memnuniyetle karşılıyoruz! 

1. Bu repo'yu fork edin
2. Feature branch oluşturun (`git checkout -b feature/YeniOzellik`)
3. Değişikliklerinizi commit edin (`git commit -m 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/YeniOzellik`)
5. Pull Request açın

## 📝 Yapılacaklar (Roadmap)

- [ ] Şablon kaydetme ve yükleme (.ptm formatı)
- [ ] Hazır şablon galerisi
- [ ] Toplu görsel işleme (batch export)
- [ ] Katman paneli (layer management)
- [ ] Daha fazla şekil seçeneği
- [ ] Gradient (renk geçişi) desteği
- [ ] Gölge efekti

## 📄 Lisans

Bu proje MIT Lisansı ile lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## 👨‍💻 Geliştirici

**Özgür Gökçe**

---

⭐ Bu proje işinize yaradıysa yıldız vermeyi unutmayın!
