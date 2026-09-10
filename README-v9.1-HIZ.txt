EĞİLMEZ v9.1 — GENEL HIZ / ADMIN ANINDA AÇILIŞ

Yapılan performans düzeltmeleri:
- Admin butonuna basınca overlay artık önce açılır; ağır ürün/döviz/hurda listeleri sonraki frame/idle sürede hazırlanır.
- Hareketli/normal mod için çalışan fazladan 2 saniyelik JSON sorgusu kaldırıldı.
- Aynı customerDisplay ayarını sorgulayan çift polling kodundan eski olan kaldırıldı.
- Firebase SSE çalışıyorsa polling kullanılmaz; SSE koparsa fallback sorgusu 2 sn yerine 8 sn.
- Üst durum DOM güncellemesi 1 sn yerine 3 sn.
- Resize işlemleri requestAnimationFrame ile tekilleştirildi.
- TV fiyat yenilemesi 2 sn olarak korunur; genel ayarlar daha seyrek sorgulanır.
- Yeni TV linki: tv.html?v=91
