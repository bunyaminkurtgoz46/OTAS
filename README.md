# DUVPAN Fabrika · Sürüm 3

Fabrikada biten imalatı, kesimi, hammadde stoğunu ve sevkiyatı (atölye → galvaniz → şantiye) takip eder.
Asıl işi: parça veya malzeme bitmeden önce uyarmak, lazerciye ve tedarikçiye zamanında haber vermek,
sevkiyatı kantar fişleriyle kayıt altına almak.

## Sürüm 3'te yeni

- **Alt menüde iki yeni sekme:**
  - **Proje:** proje listesi ve adım adım **Yeni proje** sayfası: 1) iş türü (ano / baba / serbest / benzer projeden kopya) 2) bilgiler 3) ölçüler (şemalı) 4) reçete 5) adetler ve ek sevk kalemleri 6) kontrol: kesim listesi, malzeme ihtiyacı ve stokta olup olmadığı, ağırlık, tahmini hakediş.
  - Yarım kalan proje taslağı telefonda saklanır; sonra kaldığınız yerden devam edersiniz.
  - **Reçete:** tüm reçeteler okunaklı listelenir. **Yeni reçete yaz** ile her satıra bir kalem girilir: kayıtlı parça, yeni kesilen parça (ad, malzeme, kesim boyu, nerede kesildiği, 1 boydan kaç adet çıktığı, "2'si kaynatılır") ya da kesimsiz malzeme (bütün boy).
  - 1 boydan çıkan adet ve reçete ağırlığı otomatik hesaplanır, elle değiştirilebilir. İmalat girilmiş bir reçeteyi değiştirirken uyarır; "Yeni reçete olarak kaydet" seçeneği var.

- **Kolay proje ekleme:** + Yeni proje → "Ano sistemi", "Baba sistemi" veya "Projeden kopyala".
  - Ad, uzunluk ve hat sayısını yazın; ano, bitim babası, uç, dübel, cıvata ve tonaj otomatik önerilir.
  - Önerilen sayıyı elle değiştirebilirsiniz. Değiştirdiğiniz alan bir daha otomatik değişmez; yanında "önerilen X" yazar, "Öneriye dön" ile geri alırsınız.
  - Ano kuralları: ano = toplam uzunluk ÷ ano boyu (yukarı yuvarla) · bitim babası = hat sayısı · baba = ano × 3 + bitim · dübel = baba × 4 · cıvata = (ano − hat) × 3 + %10 · uç = hat × 2.
  - Baba kuralları: baba = uzunluk ÷ aralık + köprü ek babası · boru = uzunluk × sıra ÷ 6 · dübel = baba × 4.
  - "Ano içeriğini düzenle" ile o projeye özel ano reçetesi açılır; diğer projeler etkilenmez.
  - Kesim listesi (kaç boy), malzeme ihtiyacı ve ağırlık aynı ekranda görünür.
- **Projeyi kopyala:** proje sayfasındaki düğmeyle. Ürünler, ek kalemler, şantiye sütunu ve fiyat gelir; kayıtlar gelmez.
- **Emanet aksesuar:** dübel ve cıvata galvanize korkulukla gider ama galvanizlenmez.
  - Galvaniz tablosunda "emanet" olarak görünür, galvanizde bekleyen adedi izlenir.
  - Fabrika kantarı tahminine girmez.
- **İki kantar:** şantiye sevkinde iki ayrı kilo girilir.
  - Galvaniz kantarı: sadece galvanizlenen kalemler. Toplamı galvaniz faturası kontrolü içindir.
  - Şantiye kantarı: her şey dahil. Hakediş buna göre hesaplanır.
- **Konumlu stok:** her malzeme Fabrika / Lazerci / Plazmacı olarak ayrı tutulur.
  - "Malzeme geldi"de nereye indiği seçilir.
  - "Transfer" ile yer değiştirilir (ör. fabrikadan lazerciye sac).
  - Lazer kesim lazercideki sacdan, plazma plazmacıdakinden, testere fabrikadakinden düşer.
  - Lazere kesim isterken lazercide ne kadar sac olduğu görünür.
  - Sac stoğu artık takip ediliyor.
- **Genel stok:** projeye bağlı olmayan profil, boru, sac ve aksesuarlar tutulabilir (grup, ölçü, kalınlık, not).
- **Stok kontrol paylaş:** Stok → Malzeme stoğu.
  - Gruplu liste WhatsApp'a gönderilir, kopyalanır ya da yazdırılır/PDF yapılır.
  - Gruba ve konuma göre filtrelenir; kesilmiş parçalar da eklenebilir.

## Yüklü projeler (üretim reçetelerinden)

| Proje | Durum | Üretilecek | Ek sevk kalemleri |
|---|---|---|---|
| Trabzon Makiş (REV.2) | Üretimde | 402 baba | 663 boy boru Ø88,9 (galvaniz üzerinden), 1.608 dübel |
| K.Maraş Aksu-2 (REV.1) | Sırada | 29 ano, 2 kapanış babası, 4 bükümlü uç | 356 dübel, 90 takım cıvata (emanet) |
| Osmaniye Kadirli (REV.0) | Sırada | 170 ano, 1 kapanış babası, 2 bükümlü uç | 2.044 dübel, 558 takım cıvata (emanet) |

Reçeteler:

- **1 baba** = 2 dikme sacı (lazer) + 5 manşon Ø139,7 L=150 (fabrika) + 1 flanş 297×297×15 (lazer)
- **1 ano** = 6 baba profili L80 L=1200 + 3 flanş 200×200 (lazer) + 54 dikme profili L40 L=1000 + 1 NPU100 6 m + 3 NPU80 L=1910
- **Kapanış babası** = 2 baba profili L80 + 1 flanş 200
- **Bükümlü uç** = 1 NPU100 parçası L=1500

Projenin durumu önemlidir:

- **Üretimde** olan projeler "kaç günlük kaldı" hesabına girer.
- **Sırada** olanlar sadece "ne kadar eksik" hesabına girer.

Aynı anda birden fazla proje "Üretimde" olabilir. Durumu proje sayfasının üstündeki düğmelerle tek dokunuşla değiştirin.
Aynı ürünü yapan iki proje birlikte üretimdeyse, bitiş tahmini için ürünün günlük kapasitesi projelere bölünür; projeye imalat girildikçe o projenin kendi hızı kullanılır.

## İlk iş: başlangıç sayımı

Panodaki **"Başlangıç sayımını gir"** düğmesiyle fabrikadaki parça ve malzeme miktarlarını tek ekranda girin.
Sayılmayan kalemler "Stok girilmedi" olarak görünür ve uyarı üretmez.

## Ekranlar

- **Pano:** acil uyarılar, alınacak malzeme listesi, tartım hatırlatması, eksik kantar fişleri, bugünkü imalat ve projeler
- **Stok:** üretimdeki parçalar, sıradaki işlerin parçaları ve hammadde (fabrikada ne var, ne siparişte, ne eksik)
- **Galvaniz:** fabrikadan galvanize giden seferler (her proje için hedef, giden, kalan ve fabrikada hazır olan)
- **Şantiye:** galvanizden şantiyeye giden seferler. Galvaniz ve şantiye kantarı (fiş no + kg), adetler, hat/kenar/ano no ve teslim alan kaydedilir. Hakediş tutarı da burada görünür.
- **Üst köşe:** Geçmiş (tüm kayıtlar) ve Ayarlar (ürün, parça, hammadde, yedek). Projeler panodan açılır.

## Kayıt türleri (+ düğmesi)

- Biten imalat (isteğe bağlı aşama adetleri, kişi ve tartım)
- Fabrikada kesildi (testere/plazma; hammaddeden otomatik düşer)
- Lazerden kesim geldi
- Lazere kesim iste (WhatsApp)
- Malzeme geldi (fabrikaya / lazerciye / plazmacıya)
- Malzeme transferi
- Malzeme siparişi (WhatsApp)
- Galvanize gönder
- Şantiyeye sevk
- Sayım

## Kontrol edilmesi gereken varsayımlar

Hepsi **Ayarlar**'dan değiştirilebilir:

- 6 m manşon borusundan **39 manşon** çıkıyor (150 mm + testere payı).
- Günlük kapasite: **baba 70**, **ano 12**, kapanış babası 2, uç 4. Ano kapasitesi tahmindir; gerçek imalat girildikçe ortalama hız kullanılır.
- Kesim süreleri: lazer parçaları **3 iş günü**, fabrikada kesilenler **1 iş günü**.
- Tedarik süreleri: profiller ve manşon borusu **5 iş günü**, Ø88,9 boru **7 iş günü**, dübel ve cıvata **3 iş günü**.
- Flanş 200 için plakadan kaç adet çıktığı girilmedi (sac stoğundan düşmez).
- Sac plaka ağırlıkları 6000×1510 için hesaplandı: t10 = 711,2 kg, t15 = 1.066,8 kg.
- Cıvata ağırlığı girilmedi; girilene kadar kantar tahminlerine katılmaz.
- Makiş satış fiyatı **88 TL/kg** (hakediş hesabı için). Diğer projelere fiyat girilmedi.

## Açmak ve telefona kurmak

- **Bilgisayarda:** Zip'i bir klasöre çıkarın, `index.html` dosyasına çift tıklayın.
- **Telefona:** Klasörü netlify.com'daki ücretsiz hesabınıza sürükleyip bırakın.
  - **Android:** Verilen adresi Chrome'da açıp **Telefona kur → Yükle**'ye dokunun.
  - **iPhone:** Adresi Safari'de açıp **Paylaş → Ana Ekrana Ekle**'ye dokunun.
- **APK:** pwabuilder.com'a adresi verip Android paketini indirin.

Önceki sürümü kurduysanız yeni dosyaları aynı siteye yüklemeniz yeterli. Kurulu uygulama kendini günceller; eski kayıtlar korunur.

## Önemli: şimdilik deneme modu

Kayıtlar yalnızca girildiği telefonda tutulur; formenin girdiğini ofis göremez.
Ara ara **Ayarlar → Veri → Yedeği indir** ile yedek alın.
Bir sonraki adımda ortak veritabanı bağlanacak ve herkes aynı rakamları görecek.
