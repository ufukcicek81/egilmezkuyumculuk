EĞİLMEZ KUYUMCULUK v9.0 — HIZ / PERFORMANS DÜZELTMESİ

- Admin/müşteri splash ekranı maksimum 700 ms; DOM hazırsa yaklaşık 250 ms içinde kapanır.
- Önceki aşırı sık Firebase polling aralıkları azaltıldı.
- TV fiyat sorgusu 1 sn -> 2 sn.
- TV görünüm ayarı 1.2 sn -> 3 sn.
- Genel ayarlar 2.5 sn -> 5 sn.
- Müşteri/TV config senkronları 1.5 sn civarından 4 sn civarına çıkarıldı.
- İlk TV açılışındaki ağ istekleri paralel başlatılır.
- Son TV fiyat cache sistemi korunur; açılışta son fiyat anında görünür.
- Sürekli layout hesaplama yok.
- Resize/focus işlemleri requestAnimationFrame ile tekilleştirildi.
- Yeni TV linki: tv.html?v=90
