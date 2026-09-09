EĞİLMEZ KUYUMCULUK PREMIUM v6

- Ürünler admin panelinden eklenir, silinir ve yukarı/aşağı sıralanır.
- Silinen ürün yönetim listesinden ve müşteri/TV ekranından tamamen kaybolur.
- Döviz ekleme/silme/sıralama vardır (USD, EUR, GBP, SAR, CHF canlı kaynak destekli).
- Hurda türü ekleme/silme/sıralama vardır.
- Admin ekranında Varlıklarım kaldırılmıştır.
- PC admin: Altın solda, Döviz + Hurda sağda tek ekran düzeni.
- TV: müşteri fiyat ekranı, Döviz/Hurda yok, iki kolon, başlıklar ve açık/koyu tema mevcut.
- Firebase canlı senkronizasyon ve 2 sn yedek senkron yapısı korunmuştur.

GitHub reposunda bu paketteki dosyaları kök dizine yükleyin.
Eski dosyaları silmeden önce isterseniz ayrı commit bırakın.

- v6.1: PC admin görünümü tam ekran ve ortalı hale getirildi; sağa kayma düzeltildi.

v6.2 TV düzeltmesi:
- TV ekranı artık ikiye bölünmez; müşteri ekranı gibi tek tablo kullanır.
- Birim / Alış / Satış / K. Kartı başlığı tek satır ve hizalıdır.
- Ürün eklenince/silinince TV otomatik yeniden ölçülür.
- Ürün sayısı arttıkça satır ve yazılar gerektiği kadar otomatik küçülür.
- Döviz ve Hurda TV ekranında gösterilmez.

v6.3 DONMA DÜZELTMESİ
- v6.2'deki TV otomatik sığdırma ile eski TV başlık gözlemcisinin birbirini tetiklemesi engellendi.
- Sonsuz MutationObserver döngüsü kaldırıldı.
- TV ürün sayısı değiştiğinde yalnızca bir kez yeniden ölçüm yapılır.
- Sayfa yenilemede dönme / 'yanıt vermiyor' sorunu giderildi.

v6.4 TV FINAL FIX
- renderTable tamamen sağlamlaştırıldı.
- TV başlıkları artık priceRows içine eklenmiyor.
- Yeni ürün, diğer satırlar varken de otomatik DOM'a ekleniyor.
- Silinen ürün DOM'dan tamamen çıkarılıyor.
- Sıralama her render'da doğru uygulanıyor.
- TV otomatik sığdırma DOM'a müdahale etmiyor; observer döngüsü yok.
- Birim / Alış / Satış / K. Kartı tek tablo ve tek başlık olarak hizalıdır.

v7 TV AYRI STABIL
- TV artık index.html içindeki karmaşık TV CSS/JS sistemini kullanmaz.
- TV için ayrı, temiz tv.html dosyası vardır.
- Eski ?tv=1 linki otomatik olarak tv.html?v=70 adresine yönlenir.
- Admin panelindeki TV linki artık tv.html adresini üretir.
- TV, Firebase ayarlarını ve canlı fiyatları 2 saniyede bir yeniler; sayfa refresh gerekmez.
- Ürün ekleme/silme/sıralama TV'ye otomatik yansır.
- Ürün sayısına göre yazı ve satırlar otomatik sığar.
- Döviz ve Hurda TV'de yoktur.
- Açık/Koyu tema TV'de vardır ve aynı cihazdaki tema tercihini kullanır.
