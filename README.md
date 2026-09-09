# Eğilmez Kuyumculuk Premium v5.3

Bu sürümde iki kritik stabilite düzeltmesi vardır:

- Açık/Karanlık tema tercihi cihaz bazında kalıcıdır; Firebase/admin kaydı temayı kendiliğinden değiştirmez.
- Admin değişiklikleri Firebase Realtime Database stream (SSE) ile müşteri ve TV ekranına sayfa yenilemeden anlık uygulanır. Bağlantı koparsa 2 saniyelik polling otomatik yedek olarak çalışır.

Canlı altın/döviz fiyat akışı mevcut yapıda devam eder.
