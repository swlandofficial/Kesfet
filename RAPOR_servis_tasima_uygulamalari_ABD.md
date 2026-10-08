# ABD'de Okul ve Personel Servisi Uygulamaları — Instagram Reklam Analizi

**Tarih:** 8 Ekim 2026 · **Kaynak:** Meta Reklam Kütüphanesi (ABD), Apify `apify/facebook-ads-scraper` + web araştırması
**Harcama (bu tur):** ≈ $0,43 · **Toplam Apify harcaması:** ≈ $4,77 / $5
**Ham veri:** `ham_reklam_verisi_servis_tasima.csv` (78 reklam)

## Yöntem
1. Instagram'da yayında olan reklamlar üç kelimeyle arandı: `school bus app`, `employee shuttle`, `student transportation` (her biri 22 reklam).
2. İlgisiz reklamlar elendi: oyun, dizi uygulamaları, oto bayileri, klima vb.
3. Öne çıkan 5 markanın sayfa bazında toplam/aktif reklam sayıları ve ilk reklam tarihleri çekildi. HopSkipDrive ayrıca adıyla arandı.

## Ana bulgu: Bu sektör Instagram'da tüketiciye değil, şoföre ve kurumlara reklam veriyor
Sağlık uygulamalarının aksine, servis taşıma uygulamaları Instagram'da **veliye "uygulamamı indir" reklamı vermiyor**. Bu uygulamaları **okul bölgeleri ve şirketler satın alıyor**. Instagram reklamları iki amaçla kullanılıyor:
- **Arz tarafı:** şoför ve refakatçi toplamak (Zūm, HopSkipDrive, Groome)
- **B2B:** işverenlere personel servisi satmak (Zeelo)

Türkiye'ye uyarlarken müşteri olarak veliyi ve çalışanı değil, **okulu ve işvereni** hedeflemeniz gerekir.

## Sonuç tablosu

| Uygulama | Segment | Toplam / Aktif reklam | İlk reklam | Reklam davranışı | Ne yapıyor |
|---|---|---|---|---|---|
| **Zūm** | Okul servisi (öğrenci taşıma) | **88 / 87** | 11 May 2026 | Mayıs'tan beri her ay 4–8 yeni reklam açıyor, neredeyse hiç kapatmıyor (88'in 87'si açık). Reklamlar şoför alımı için: "$21/saat, sağlık sigortası, 401k". | Okul bölgelerine yapay zekâ destekli rota planlama, elektrikli okul otobüsü ve veliye canlı takip uygulaması sunuyor. Okul bölgesiyle sözleşme yapıp yeni bölgelere açıldıkça şoför arıyor. |
| **HopSkipDrive** | Okul servisi (özel ihtiyaçlı ve barınma desteği alan öğrenciler, küçük araç) | ≥12 aktif | 14 Ağu 2026 | Okul döneminin başında 12 reklam açılmış, hepsi açık. Reklamlarda "CareDriver" ve refakatçi aranıyor. | Sarı otobüsün gidemediği öğrencileri (IEP, McKinney-Vento kapsamındakiler) küçük araçlarla taşıyor. 13.500'den fazla okul, 5 milyondan fazla yolculuk. 2026-27 dönemi için tüm yolculuklarda ücretsiz video kaydı ve "her gün aynı şoför" programı başlattı. |
| **Zeelo** | Personel servisi (ev-iş, vardiya) | 22 (2 sayfa) / 15 | Haz 2026 | **Yeni bir reklam formatı:** "Maeve" ve "Emma" adlı **AI/persona "ulaşım uzmanı" sayfaları** açmış ve aynı mesajı bu sayfalardan veriyor: "Güvenilir servis işe devamı artırır, bana sorun!" Maeve sayfasının tüm reklamları son 11 günde açılmış, ölçekleniyor. | İngiltere kökenli, ABD'de hızla büyüyor. Rota ve bilet uygulaması, şoför uygulaması ve işveren paneli var. 15 milyon yolculuğun 5 milyonu son 10 ayda yapılmış. Müşterilerinde 90 günlük çalışan tutma oranında %30 artış iddia ediyor. |
| **AngelSense** | Veli (özel ihtiyaçlı çocuk) | 26 / 20 | 2023 | 2023'ten beri açık bir reklamı var, yani kârlı. **Ekim 2026'da 17 yeni reklam açılmış.** Ana hikâye: "Otizmli oğlum okul servisinde unutuldu…" | Servis değil, çocuğa takılan GPS + dinleme cihazı. Ama reklamı doğrudan **okul servisi korkusu** üzerine kurulu. Velinin servise güvenmediğini gösteren güçlü bir talep sinyali. |
| Groome, Nooga Shuttles, Rohrer Bus, BTI | Klasik taşıma firmaları | — | — | Şoför alımı ya da yerel tanıtım reklamları. | Uygulama değil, operatör. |

## Türkiye için öneriler

### 1. Zūm / HopSkipDrive modeli → "Okul servisi yönetim platformu"
- **Pazar:** Türkiye'de okul servisini çoğunlukla bağımsız servisçiler yapıyor ve veliyle WhatsApp üzerinden iletişim kuruyorlar. Canlı konum, "araç kapıda" bildirimi, yoklama (çocuk bindi/indi) ve **"araçta çocuk unutuldu" alarmı** büyük bir boşluk. Türkiye'de her yıl servis aracında çocuk unutulma haberleri çıkıyor; AngelSense'in reklam hikâyesi bunun ne kadar güçlü bir motivasyon olduğunu gösteriyor.
- **Müşteri:** Özel okullar ve kolej zincirleri (B2B). Veli uygulamayı ücretsiz kullanır, servisçi ve okul abonelik öder.
- **Reklam stratejisi:** Velilere duygusal hikâye (AngelSense tarzı), okul yöneticilerine LinkedIn/Instagram B2B mesajı, servis şoförlerine "daha çok rota, düzenli ödeme".
- **Mevzuat:** Okul servis araçları yönetmeliği (rehber personel ve araç şartları) ile KVKK kapsamında **çocuk konum verisi** işlenmesi dikkat gerektirir.

### 2. Zeelo modeli → "Personel servisi için rota + rezervasyon uygulaması"
- Türkiye'de OSB'lerde ve fabrikalarda personel servisi çok yaygın ama genellikle kâğıt listeyle ve sabit rotayla yönetiliyor.
- **Değer önerisi:** Hibrit çalışma ve vardiya için koltuk rezervasyonu, dinamik rota, doluluk raporu ve "servis kaçırdım" sorununun çözümü.
- **Satış argümanı:** Zeelo'nun ana mesajı "işe devam ve çalışan tutma oranı". Türkiye'de mavi yaka sirkülasyonu yüksek olduğu için aynı argüman güçlü çalışır.
- **Reklam fikri:** Zeelo'nun "persona uzman" sayfası (Maeve/Emma) taktiği Türkiye'de de denenebilir. Örneğin "Servis Uzmanı Ayşe" adlı bir sayfadan İK müdürlerine reklam verilebilir.

## Sınırlamalar
- Bütçe kısıtı nedeniyle her aramada yalnızca 22 reklam çekildi.
- **Bu alanda Instagram iyi bir sinyal kaynağı değil:** Satın alma kararı okul bölgesinde ve İK'da veriliyor. Bu alanda LinkedIn reklamları ve okul bölgesi ihale kayıtları daha anlamlı veri verir.
- Meta, ABD ticari reklamları için harcama verisi vermiyor. Değerlendirme reklamların ne kadar süre açık kaldığına ve yeni reklam açılma hızına dayanıyor.
- Zūm'ün ürün açıklaması kendi kamuya açık tanıtımına dayanıyor. Bu turda Zūm hakkında ayrıca güncel haber araması yapılmadı.

## Kaynaklar
- [HopSkipDrive – 2026-27 ücretsiz yolculuk kaydı ve sabit şoför programı (STN)](https://stnonline.com/industry-releases/hopskipdrive-brings-free-ride-recording-and-consistent-caredriver-program-to-2026-2027-school-year/)
- [HopSkipDrive – okul ortaklıkları %35 arttı](https://www.hopskipdrive.com/blog/growing-our-school-partnerships-by-35-as-we-prepare-for-our-biggest-back-to/)
- [HopSkipDrive – 6 yeni eyalete genişleme (Business Wire)](https://www.businesswire.com/news/home/20250818096273/en/HopSkipDrive-Plans-Expansion-Across-Six-New-States-for-the-2025-2026-School-Year)
- [BusRight $30M yatırım (School Bus Fleet)](https://www.schoolbusfleet.com/news/busright-raises-30m-to-enhance-platform-features)
- [Zeelo – personel servisi](https://zeelo.co/employee-shuttles) · [Zeelo blog](https://zeelo.co/blog)
- [Goryde – personel servisi yazılımı rehberi 2026](https://goryde.com/blog/best-employee-shuttle-management-software-2026/)
- Meta Reklam Kütüphanesi page_id: Zūm 772048659588555, HopSkipDrive 103480144441214, Zeelo (Maeve) 774882942366436, Zeelo (Emma) 514941971713781, AngelSense 1417537291824671
