# Türkiye'de Zūm Benzeri Okul Servisi Platformu — Rakip ve Pazar Analizi

**Tarih:** 9 Ekim 2026 · **Yöntem:** Web araştırması, MEB yönergesi ve teknik şartnamesi, rakiplerin siteleri ve haberler (Apify kullanılmadı)

## Kısa cevap

1. **Türkiye'de Zūm'ün birebir benzeri yok.** Zūm bir **taşıma operatörü**: kendi araç ve şoför ağı, yapay zekâ ile rota planlama, elektrikli otobüsler ve okul bölgeleriyle doğrudan sözleşmeler. Türkiye'de servis işini binlerce bağımsız **servis esnafı** yapıyor ve piyasa esnaf odalarıyla belediye düzenlemelerine bağlı. Bu yüzden Zūm gibi bir operatör kurmak Türkiye'de çok zor.
2. **Zūm'ün yazılım tarafının benzerleri ise çok:** canlı konum, bindi/indi bildirimi, veli uygulaması, rota ve tahsilat. Bu alanda en az 10 rakip var. Pazar kalabalık ve bu hizmet artık sıradanlaştı.
3. **Devlet de oyuna girdi:** MEB, taşımalı eğitim için merkezi bir takip sistemi kurdu ve özel tedarikçileri lisanslıyor.
4. **Sonuç:** "Bir servis takip uygulaması daha" yaparsanız rakiplerle fiyat üzerinden yarışırsınız ve zorlanırsınız. **Belirli bir niş seçip donanımsız, ucuz ve tam operasyon çözümü sunarsanız** yarışabilirsiniz (bkz. bölüm 5).

## 1. Pazar yapısı

| Segment | Parayı kim ödüyor | Durum |
|---|---|---|
| **Taşımalı eğitim** (MEB'in köy ve mahallelerden merkez okullara taşıdığı öğrenciler) | Devlet (ihale ile taşıyıcıya) | MEB'in 22.07.2025 tarihli yönergesiyle **dijital takip zorunlu**. Yaklaşık 1 milyon öğrenci (2026 haberleri). |
| **Özel okul ve kolej servisleri** | Veli (servis ücreti) → okul veya servis firması | MEB yönergesinin **kapsamı dışında**. Okullar ve servis firmaları kendi tercih ettikleri yazılımı kullanıyor. |
| **Devlet okullarına velinin anlaştığı servisler** | Veli, servisçiye doğrudan | En dağınık ve en dijitalleşmemiş segment. Genellikle WhatsApp grubuyla yönetiliyor. |

**Araç sayısı:** Türkiye'de 70 bin ile 340 bin arası servis aracı olduğu söyleniyor (2008 ve 2020 tarihli, birbiriyle çelişen tahminler). İstanbul'da yaklaşık 20 bin okul servisi var.

**Mevzuat:**
- Okul Servis Araçları Yönetmeliği araç takip sistemi ve kamera istiyor. Eski model araçlar için geçiş süreleri 2026–2028 arasında değişiyor.
- İBB UKOME, İstanbul'da okul servislerine kamera zorunluluğu kararı aldı.

## 2. MEB'in sistemi — en önemli rekabet unsuru

"Öğrenci Servisi Planlama, Takip, Kontrol, Bilgilendirme ve Yönetim Sistemi Yönergesi" (MEB DHGM, 22.07.2025):

- **Kapsam:** Yalnızca *Taşıma Yoluyla Eğitime Erişim Yönetmeliği* kapsamındaki servis araçları, yani taşımalı eğitim (Madde 2). **Özel okul servislerini kapsamıyor.**
- **Model:** MEB tek bir yazılım yapmıyor. Uygunluk başvurusunda bulunan **birden fazla özel tedarikçiyi yetkilendiriyor.**
  - Uygunluk belgesi 3 yıl geçerli. ISO/IEC 27001 belgesi ve sızma testi raporu isteniyor.
  - Tedarikçinin yazılımı **"Bakanlık çatı yazılımına" entegre olmak zorunda** (Madde 15/7).
- **Veliden ücret alınamaz:** Bildirimler (SMS, sesli arama, uygulama) "kullanıcıdan herhangi bir ücret talep edilmeksizin" verilmeli. Masrafı taşıyıcı (servisçi) üstleniyor.
- **İstenen özellikler:**
  - Konum, hız, rota, kapı hareketleri
  - Bindi/indi yoklaması
  - Şoför, veli, rehber personel ve okul uygulamaları
  - Numarasız (maskeli) arama
  - Biyometrik şoför doğrulaması (ertelendi)
- **Belirli bir cihaz şartı yok:** MEB'in Eylül 2025 duyurusuna göre "araç takip cihazı" adıyla belirli bir donanım zorunlu değil. İstenen fonksiyonları yerine getiren **yazılım veya modül de kabul ediliyor.**
- **Tartışma:** Servis esnafı, cihaz ve yazılım için **12–30 bin TL** maliyetten şikâyet ediyor. Trabzon'da "piyasada 2-3 bin TL olan cihaz 23 bin TL'ye aldırılıyor" iddiası var. Bir milletvekili, sistemin tek firmaya (Turkcell) yönlendirildiği iddiasıyla soru önergesi verdi.

**Ne anlama geliyor?**
- **Taşımalı eğitim:** Yetkilendirilmiş tedarikçi olmak bir kamu (B2G) fırsatı. Ama süreç bürokratik, segment siyasi ve fiyata çok duyarlı.
- **Özel okul segmenti:** Serbest. Ancak velilerin beklentisini MEB sistemi belirleyecek: canlı takip, yoklama ve maskeli arama her serviste olması gereken asgari özellikler hâline geliyor.

## 3. Rakipler

| Rakip | Ne yapıyor | Hedef müşteri | Güçlü yanı | Zayıf yanı |
|---|---|---|---|---|
| **Serviscell** (Turkcell; App Store'da geliştirici Polar Teknoloji) | Canlı takip, bindi/indi, sesli arama ve SMS bildirimi, maskeli arama, kamera. 2016'dan beri var. | Okul + servis firması (araç başına lisans) | Marka, operatör gücü, MEB sistemine en hazır görünen oyuncu | Pahalı olduğu ve esnafa dayatıldığı yönünde tepki var. Eski ürün. |
| **okulservisi.net** | Öğrenci/veli yönetimi, **aidat tahsilatı**, rota, canlı takip, SMS, KVKK araçları. 14 gün ücretsiz deneme. | **Servis firmaları** | Operasyon ve tahsilat odaklı | Müşteri sayısı belirsiz. MEB entegrasyonu iddiası yok. |
| **tasimaliegitim.com** | Taşımalı eğitime yönelik takip ve mevzuat içerikleri | Taşımalı eğitim taşıyıcıları | Niş içerik ve SEO | — |
| **Servis Konum** (serviskonum.com) | Okul/firma, şoför, veli ve yolcu uygulamaları, yaklaşma uyarısı | Okul + firma | Okul ve personel servisi birlikte | — |
| **Okul Yolum** (okulyolum.net) | Canlı takip, SMS ve arama bildirimi | Anaokulu ve kreşler | Niş | Uygulaması 2019'dan beri güncellenmemiş görünüyor |
| **iOkul**, **Hürsoft**, **Zeymus**, **ogrencitasimaciligiprogrami.com** | Servis takip modülleri | Okul + firma | — | Klasik yazılım firmaları |
| **Onlibüs** | Veli takibi, otomatik yoklama, adres değişikliği. Planlananlar: yapay zekâ ile rota optimizasyonu, şoför performansı | Okul + servis firması | Yapay zekâ vizyonu. BTM yatırımı ve TÜBİTAK 1512 desteği aldı. | 2022'den beri pilot aşamada (9 kurum, ~2.000 öğrenci) |
| **Okulyo** (dolaylı rakip) | Okul yönetimi + **servis ve kantin ödemeleri** | Okullar | Aralık 2025'te Insha GSYF'den yatırım aldı | Servis takibi ana odağı değil |
| **Filo takip firmaları** (Arvento, Mobiliz vb.) | GPS donanımı ve filo takibi | Büyük servis firmaları | Donanım ve ölçek | Veli deneyimi zayıf |
| **MEB çatı sistemi** | Merkezi takip + tedarikçi entegrasyonu | Taşımalı eğitim | Zorunlu ve ücretsiz bilgilendirme | Sadece taşımalı eğitim |

## 4. Zūm gibi bir proje Türkiye'de yarışabilir mi?

| Seçenek | Rekabet | Yarışabilir mi? |
|---|---|---|
| **A. Zūm gibi operatör olmak** (kendi araç ve şoför ağı) | Esnaf servisçiler, odalar, S plaka ve güzergâh izinleri, belediye tarifeleri | **Zor.** Çok sermaye ister, düzenleme engeli var ve esnaf tepki gösterir. Önerilmez. |
| **B. Bir servis takip uygulaması daha** | En az 10 rakip + MEB'in ücretsiz bilgilendirme şartı | **Zayıf.** Sıradan bir ürün olursunuz ve fiyat savaşına girersiniz. |
| **C. Niş bir segment için tam operasyon platformu** (aşağıda) | Rakiplerin çoğu sadece takip yapıyor | **Evet, yarışabilir.** |

## 5. Önerilen konumlandırma: "Özel okullar ve kolej zincirleri için yapay zekâ destekli servis operasyon platformu"

Zūm'ün asıl değeri takip değil, **operasyonu verimli hâle getirmek**. Türkiye'de boş kalan alan da tam burası.

1. **Donanımsız (sadece telefon) kurulum:** MEB bile belirli bir cihaz zorunluluğunu kaldırdı ve yazılımsal çözümleri kabul ediyor. Esnafın 12–30 bin TL'lik cihaz şikâyeti sizin için bir satış argümanı: **"Cihaz yok, şoförün telefonu yeter."**
2. **Yapay zekâ ile rota ve araç optimizasyonu:** Yeni dönem kayıtlarında adresleri otomatik kümeleyip "bu okul 42 yerine 36 araçla çalışabilir" raporu çıkarmak. Bu, okul için doğrudan para tasarrufu demek ve rakiplerde yok (Onlibüs yalnızca planlıyor).
3. **Servis ücreti tahsilatı ve hakediş:** Veli ödemesi → okul → servisçi. Tahsilat, gecikme takibi, iade. okulservisi.net ve Okulyo bu tarafı yapıyor; siz bunu rota ve takip ile tek pakette birleştirirsiniz.
4. **Mevzuat paketi:** Okul Servis Araçları Yönetmeliği belgeleri, araç yaşı, muayene, rehber personel, şoför belgesi ve kamera kaydı takibi. Denetim günü için tek tıkla rapor.
5. **Güven özellikleri:** Bindi/indi yoklaması, **"araçta çocuk kaldı" kontrolü** (son durakta şoförün araç içini kontrol ettiğini onaylaması), maskeli arama, KVKK'ya uygun açık rıza akışları.
6. **İkinci aşama:** MEB uygunluk belgesi için başvurup taşımalı eğitime de girmek. Ürün baştan MEB teknik şartnamesindeki işlevlere ve çatı yazılım entegrasyonuna uygun tasarlanmalı.

**Gelir modeli:** Okul başına **öğrenci başı yıllık lisans** (kolej zincirleriyle toplu anlaşma), tahsilattan küçük bir komisyon ve servis firmalarına araç başı aylık ücret. Veli uygulaması ücretsiz olmalı (MEB normu da bu yönde).

**İlk hedef müşteri:** Kolej zincirleri. Yüzlerce aracı tek merkezden yönetiyorlar ve servis şikâyetleri veli memnuniyetini doğrudan etkiliyor. Zincir olmayan özel okullar ikinci sırada gelir.

## 6. Riskler
- **Turkcell/Serviscell'in dağıtım gücü:** Operatörün paket indirimleri ve kurumsal ilişkileri güçlü.
- **Servis esnafının direnci:** Yeni maliyet ve denetim kaygısı var. Şoför tarafında uygulama **ücretsiz ve kolay** olmalı.
- **MEB kapsamının genişleme ihtimali:** Sistem ileride özel okul servislerine de uzatılabilir. O zaman uygunluk belgesi şart olur. Ürünü baştan şartnameye uygun kurmak bu riski fırsata çevirir.
- **KVKK:** Çocukların konum verisi özel dikkat gerektirir. Açık rıza, veri saklama süresi ve erişim kayıtları baştan tasarlanmalı.
- **Doğrulanamayan bilgiler:**
  - MEB'in yetkilendirdiği tedarikçilerin güncel listesi bulunamadı (DHGM sitesinde yayımlanacağı belirtiliyor).
  - Cihaz fiyatı ve "tek firma" iddiaları doğrulanmamış haber ve iddialar.
  - 2026-27 taşıma ihalesi örnek idari şartnamesinde takip sistemi şartı açıkça bulunamadı.

## Kaynaklar
- [MEB DHGM – Dijital takip sistemi duyurusu (24.07.2025)](https://dhgm.meb.gov.tr/www/ogrenci-tasima-hizmetlerinde-yeni-donem-dijital-takip-ve-yonetim-sistemi-hayata-geciriliyor/icerik/1146)
- [MEB – Yönerge metni (PDF)](https://mevzuat.meb.gov.tr/dosyalar/2289.pdf) · [Teknik şartname (PDF)](https://dhgm.meb.gov.tr/meb_iys_dosyalar/2025_08/06162013_tekniksartname.pdf) · [Sistem tedarikçilerine duyuru](https://dhgm.meb.gov.tr/www/sistem-tedarikcilerine-duyuru/icerik/1150)
- [MEB – Taşımalı eğitimde dijital takip dönemi başladı](https://www.meb.gov.tr/tasimali-egitim-hizmetinde-dijital-takip-donemi-basladi/haber/37880/tr)
- [Merkezefendi Haber – Okul servislerine Serviscell yükü (16.04.2026)](https://merkezefendihaber.com.tr/okul-servislerine-serviscell-yuku/)
- [Haber61 – Trabzon'da servisçi esnafının takip cihazı tepkisi](https://www.haber61.net/trabzon/trabzonda-servisci-esnafindan-takip-cihazi-tepkisi-piyasadaki-fiyatin-4-h625781.html)
- [Sözcü – Kamera zorunluluğu ertelemesi](https://www.sozcu.com.tr/okul-servislerinde-tacizlere-karsi-getirilen-onlemler-ertelendi-wp7289374) · [Medyascope – İstanbul'da kamera zorunluluğu](https://medyascope.tv/2025/09/25/istanbulda-okul-servis-araclarina-kamera-zorunlulugu-geldi/)
- Rakipler: [Serviscell](https://www.serviscell.com.tr/) · [Serviscell lisanslama](https://www.serviscell.com.tr/uyelik.html) · [okulservisi.net](https://okulservisi.net/) · [Servis Konum](https://www.serviskonum.com/) · [Okul Yolum](https://okulyolum.net/) · [iOkul](https://iokul.com/servis.html) · [tasimaliegitim.com](https://tasimaliegitim.com/users/okul-servisi-takip) · [Zeymus](https://zeymus.com/okul-servis-takip-mobil-uygulamasi/) · [Hürsoft](https://www.hursoft.net/sayfa/okul-ogrenci-servis-arac-takip-sistemi) · [Öğrenci Taşımacılığı Programı](https://ogrencitasimaciligiprogrami.com/servistakip.aspx)
- [İstanbul Ticaret Gazetesi – Onlibüs](https://istanbulticaretgazetesi.com/okul-servislerini-akillandiran-uygulama) · [Webrazzi – Okulyo yatırımı](https://webrazzi.com/2025/12/29/egitim-teknolojilerine-odaklanan-okulyo-insha-gsyf-den-yatirim-aldi/)
- [Hürriyet – 70 bin okul servisi](https://www.hurriyet.com.tr/gundem/turkiye-de-70-bin-okul-servisi-cocuklarimizi-gelecege-tasiyor-9700991) · [AA – servis araç sayısı](https://www.aa.com.tr/tr/turkiye/ogrenciler-okullar-kapanana-kadar-servisin-ayni-koltugunda-oturacak/1967491) · [TRT Haber – İstanbul 20 bin servis](https://www.trthaber.com/haber/turkiye/istanbulda-yaklasik-20-bin-okul-servisi-yollara-cikmaya-hazirlaniyor-429460.html)
