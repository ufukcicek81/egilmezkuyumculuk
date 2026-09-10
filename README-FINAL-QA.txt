EĞİLMEZ KUYUMCULUK v8.7 FINAL QA

KONTROL EDİLEN / DÜZELTİLENLER
- Admin, müşteri ve TV: açık mod beyaz/nötr gri; kahverengi-krem kenar kalıntıları kaldırıldı.
- Alış kırmızı, Satış yeşil, K.Kartı mavi; Has Alış kırmızı, Has Satış yeşil.
- PC admin ve müşteri: 70/30 Altın + Döviz/Hurda düzeni.
- Döviz ve Hurda artık gerçek ayrı kart wrapper'ları kullanıyor; başlık/kolon/satırların farklı yerlere kaçması önlendi.
- Müşteri Döviz/Hurda opsiyonları bütün kartı gizler; yalnız satırları değil.
- TV Döviz/Hurda opsiyonları Firebase /tvDisplay üzerinden canlı senkron.
- Müşteri opsiyonları Firebase /customerDisplay üzerinden canlı senkron.
- Farklı admin cihazları ayar değişikliklerini buluttan yeniler.
- PC ekran yüksekliğine göre altın ve yan panel satır/yazı ölçüsü otomatik sığdırılır.
- TV sayfası temiz tek CSS/JS yapısındadır; layout polling yok, titreme yapmaz.
- TV 100vw x 100vh içine sığar; scroll yok.
- TV'de adminin Döviz/Hurda ekleme-silme-sıralaması settings.dovizItems / settings.hurdaItems üzerinden aynen takip edilir.
- Ürün ekleme-silme-sıralama korunur.
- Döviz ekleme-silme-sıralama korunur.
- Hurda ekleme-silme-sıralama korunur.
- Admin ekranında Varlıklarım görünmez; müşteri tarafındaki Varlıklarım korunur.
- Service Worker network-first / no-store yapısında; eski cache temizlenir.
- Cache sürümleri v87 olarak yenilendi.

YÜKLEME
ZIP içindeki bütün dosyaları repo köküne yükleyin.
Özellikle index.html, admin.html, tv.html, manifest.json, manifest-admin.json ve sw.js birlikte güncel olmalı.
Yeni TV bağlantısı: tv.html?v=87
