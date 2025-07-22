# Ultimate Trend Confirmation System (UTCS) Pro v5.0

![Lisans](https://img.shields.io/badge/lisans-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-TradingView-brightgreen.svg)
![Sürüm](https://img.shields.io/badge/sürüm-v5.0-orange.svg)

UTCS Pro v5.0, piyasa gürültüsünü filtreleyerek yatırımcılara yüksek olasılıklı giriş sinyalleri sunmak için tasarlanmış, çok katmanlı bir onay mekanizmasına sahip, hepsi-bir-arada bir TradingView ticaret sistemidir.

![UTCS Pro v5.0 in Action](https://r.resimlink.com/BUDjyQC8.png)

---

## 📜 Özet

UTCS Pro v5.0, basit bir trend indikatörünün çok ötesindedir. Temel amacı, bir trendin hem başlangıcını hem de devamlılığını tespit ederek, bunu çeşitli filtrelerle onaylayarak ve kullanıcıya esnek strateji seçenekleri sunarak isabet oranını artırmaktır. Sistem, hem manuel işlem yapanlar için görsel bir rehber hem de otomatik sistemler için güçlü bir sinyal üreticidir.

---

## 🚀 Ana Özellikler

* **Çoklu Onay Filtreleri:** Bir sinyalin gücünü ölçmek için İkincil Uzun Vadeli EMA, ADX (Trend Gücü), RSI (Momentum) ve Hacim gibi kritik filtreleri kullanır.
* **Trend Başlangıç ve Devam Sinyalleri:** Sadece trendin başladığı yeri büyük **"BAŞLA"** etiketleriyle göstermekle kalmaz, aynı zamanda devam eden bir trend içindeki geri çekilmelerden sonra küçük oklarla (**▲▼**) yeniden giriş fırsatları sunar.
* **Gelişmiş Gösterge Panelleri:**
    * **Çoklu Zaman Dilimi (MTF) Paneli:** Farklı zaman dilimlerindeki trend yönünü tek bakışta görmenizi sağlar.
    * **Sistem Kontrol Paneli:** Ana trendin ve tüm filtrelerin anlık durumunu göstererek piyasanın genel sağlığı hakkında bilgi verir.
* **Otomasyona Hazır Alarmlar:** Ürettiği tüm sinyaller için, 3. parti otomasyon servisleriyle (trading botları vb.) kolayca entegre edilebilen, zengin içerikli **JSON formatında** alarmlar oluşturur.
* **Esnek Onay Modları:** Yatırımcının risk iştahına ve piyasa koşullarına göre stratejisini anında adapte etmesine olanak tanıyan 3 farklı çalışma modu sunar.

---

## ⚙️ Temel Konsept: Nasıl Çalışır?

İndikatörün kalbinde, fiyata çok hızlı tepki veren bir **ZLEMA (Sıfır Gecikmeli Üstel Hareketli Ortalama)** ve bu ortalamanın etrafına çizilmiş volatilite bantları bulunur. Ana sinyal, fiyatın bu bantların dışına çıkarak güçlü bir momentum ve potansiyel bir trend değişimi gösterdiği anda tetiklenir. Sistemin asıl gücü ise bu ham sinyali, seçilen **Onay Modu**'na göre çeşitli testlerden geçirmesidir.

---

## 📈 TradingView'e Ekleme

1.  TradingView'de grafiğinizi açın ve alt paneldeki **"Pine Editörü"** sekmesine tıklayın.
2.  Editördeki mevcut kodları silin.
3.  Bu repodaki `UTCS-Pro-v5.0.pine` dosyasının içeriğinin tamamını kopyalayın.
4.  Kopyaladığınız kodu Pine Editörü'ne yapıştırın.
5.  Editörün üst kısmındaki **"Kaydet"** butonuna tıklayın ve ardından **"Grafiğe Ekle"** butonuna basın.

---

## 🛠️ Yapılandırma: Sinyal Onay Modları

UTCS Pro v5.0, 3 temel onay modu sunar. Bu modlar, indikatör ayarlarından kolayca değiştirilebilir:

### 1. Esnek (Sadece Ana Trend)

* **Açıklama:** En hızlı ve filtresiz mod. Sadece ZLEMA bandı kırılımını dikkate alır.
* **Kullanım Alanı:** Yüksek risk iştahına sahip, piyasayı yakından takip eden ve hızlı hareket etmek isteyen agresif trader'lar için uygundur.

### 2. Dengeli (Ana + İkincil Trend)

* **Açıklama:** Varsayılan ve en çok tavsiye edilen mod. Ana sinyali, uzun vadeli trendi gösteren İkincil EMA (varsayılan 200 periyot) ile teyit eder.
* **Kullanım Alanı:** Güvenlik ve hız arasında mükemmel bir denge kurar. Trendin tersine işlem yapma riskini büyük ölçüde azaltır.

### 3. Katı (Tüm Filtreler)

* **Açıklama:** En muhafazakar ve en güvenli mod. Bir sinyalin geçerli olması için İkincil EMA, ADX, RSI ve Hacim filtrelerinin **tamamından** onay alması gerekir.
* **Kullanım Alanı:** Daha geç ama çok daha isabetli sinyaller üretir. Özellikle yatay piyasalardaki yanlış sinyallerden korunmak için idealdir.

---

## 👨‍💻 Geliştiriciler İçin

### Hata Bildirimi

Eğer bir hata bulursanız veya bir sorunla karşılaşırsanız, lütfen bu repo altında bir **"Issue"** açmaktan çekinmeyin.

### Katkıda Bulunma

Katkılarınız bizim için değerlidir. Projeyi geliştirmek için "fork" edebilir ve "pull request" gönderebilirsiniz. Lütfen kodlama stilini mevcut projeyle tutarlı tutmaya özen gösterin.

---

## 📝 Lisans

Bu proje, MIT Lisansı altında lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakınız.

---

## ⚠️ Sorumluluk Reddi

Bu proje yalnızca eğitim ve araştırma amaçlıdır. Finansal bir tavsiye değildir. Bu indikatörü kullanarak yapacağınız işlemlerin tüm sorumluluğu size aittir. Geçmiş performans, gelecekteki sonuçların garantisi değildir. Lütfen yatırım kararlarınızı alırken kendi araştırmanızı yapın ve riskinizi yönetin.
