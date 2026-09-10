EĞİLMEZ KUYUMCULUK v8.2 — TEK SEFERLİK SENKRON DÜZELTME

1. TV Döviz/Hurda ayarı artık ana ayar nesnesinden bağımsız bir Firebase düğümünde tutulur:
   /tvDisplay
   Bu sayede farklı admin cihazları eski ayarları birbirinin üstüne yazamaz.

2. Admin'de TV Döviz/Hurda anahtarına dokunulduğu anda Firebase'e yazılır.
   Kaydet butonuna basmayı beklemez.

3. Tüm açık admin ekranları TV ayarlarını 1.5 saniyede bir buluttan yeniler.
   Başka cihaz kapattığında açık olan diğer admin ekranındaki buton da kendiliğinden değişir.

4. TV ekranı /tvDisplay ayarını 1 saniyede bir kontrol eder.
   Döviz/Hurda kapatıldığında sayfa yenilemeden kaybolur.
   İkisi de kapalıysa Altın paneli otomatik tam genişliğe geçer.

5. Açık mod arka planları bütün ekranlarda beyaz/nötr gri yapıldı.
   Kahverengi/krem zeminler kaldırıldı.
   Admin, müşteri ve TV aynı beyaz görsel dile sahiptir.

6. Has Alış kırmızı, Has Satış yeşil.
   Alış kırmızı, Satış yeşil, K.Kartı mavi düzeni korunur.

KURULUM:
ZIP'in tamamını GitHub repo köküne yükleyin.
index.html + admin.html + tv.html birlikte güncellenmelidir.
