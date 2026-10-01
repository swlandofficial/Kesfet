# Japonya & Güney Kore — Sağlık Uygulamaları Instagram Reklam Analizi

**Tarih:** 1 Ekim 2026 · **Kaynak:** Meta Reklam Kütüphanesi (Instagram'da yayında olan reklamlar), Apify `apify/facebook-ads-scraper`
**Harcama (bu tur):** ≈ $1,07 · **Toplam Apify harcaması:** ≈ $4,29 / $5
**Ham veri:** `ham_reklam_verisi_japonya_kore.csv` (180 reklam)

## Yöntem

| Ülke | Aranan kelime (yerel dilde) | Anlamı |
|---|---|---|
| Japonya | オンライン診療 | online muayene |
| Japonya | 健康 アプリ | sağlık uygulaması |
| Japonya | 介護 アプリ | bakım uygulaması |
| G. Kore | 비대면 진료 | yüz yüze olmayan (uzaktan) muayene |
| G. Kore | 건강 앱 | sağlık uygulaması |
| G. Kore | 병원 앱 | hastane uygulaması |

Her aramada 30 aktif reklam çekildi. Sonra öne çıkan 6 markanın sayfasındaki **toplam ve aktif reklam sayıları** ile **ilk reklam tarihleri** alındı.
Japonya'da online muayene reklamlarının çoğu AGA (saç dökülmesi), ED, doğum kontrol hapı ve diyet ilacı kliniklerine ait. Kore'de ise kore tıbbı (한의원) diyet ilacı reklamları baskın. Bunlar uygulama değil klinik reklamı olduğu için elendi. Köklü markalar (Gangnam Unni, Luna Luna, Oura, Flo) da yalnızca referans olarak alındı.

## Sonuç tablosu

| Uygulama | Ülke | Kim kullanıyor | Toplam / Aktif reklam | İlk reklam | Reklam davranışı |
|---|---|---|---|---|---|
| **カイテク Kaitech** — bakım/hemşirelik için tek seferlik vardiya uygulaması | JP | **Hemşire, bakıcı + bakım kurumları** | 48/48 + 9/9 (2 sayfa) | 28 Ağu 2026 | 10 Eylül'den beri bir ayda 48 reklam açılmış, hiçbiri kapanmamış. **Bütçeyi şu anda hızla artırıyor.** 1,41 milyon sağlık profesyoneli ve 32 bin kurum kullanıyor. |
| **붐케어 Boomcare / 다다닥 Dadadoc** — bebek-çocuk için akıllı termometre + uzaktan muayene | KR | **Ebeveyn (hasta yakını)** | 39 / 38 | 29 Tem 2026 | Temmuz–Ağustos'ta 4 test reklamı açılmış. **Eylül'de 26 yeni reklamla ölçeklemeye geçmiş.** Kapanan tek reklam 8 günde kapatılmış (kaybeden test). |
| **나만의닥터 My Doctor** — uzaktan muayene + ilaç/eczane fiyat karşılaştırma | KR | Hasta | Influencer hesaplarından (≥10 reklam) | Ağu–Eyl 2026 | Kore'nin 1 numaralı uzaktan muayene uygulaması (Ocak–Ağustos 2026 boyunca MAU'da 1.), 3 milyon üye. Reklamlarda "akne muayenesi 15.000 ₩ yerine 2.300 ₩" ve "Mounjaro'nun en ucuz eczanesi" vaatleri var. |
| **모두닥 Modoodoc** — hastane/klinik yorum + fiyat karşılaştırma + randevu | KR | Hasta | **71 / 71** | 26 May 2026 | Mayıs'tan beri açtığı **71 reklamın hepsi açık** → reklamlar kârlı. Reklamda "2025'te rezervasyonda 1 numara" diyor. |
| **パシャっとカルテ Pasha-tto Karte** — tahlil/check-up sonucu ve reçeteyi fotoğrafla kaydetme | JP | Hasta + aile | 16 / 16 | 27 Tem 2026 | Temmuz'dan beri açtığı reklamların hepsi açık. Küçük ama istikrarlı büyüyor. |
| **필라이즈 Pillyze** — AI beslenme/sağlık takibi (GLP-1 kullananlara yönelik) | KR | Hasta | 17 / 17 | 25 Ağu 2026 | Eylül'de 15 yeni reklam açılmış; influencer'lara özel indirim kodu kullanıyor. |
| Upmind — telefon kamerasıyla otonom sinir sistemi ölçümü | JP | Kullanıcı | 14 aktif (tarama) | ~3 yıl önce | **1.131 gündür açık bir reklamı var**, yani uzun süredir kârlı. Ama artık yeni bir uygulama değil. |

## Türkiye için en iyi 2 aday

### 1. Kaitech → Türkiye'de "hemşire ve bakıcı için tek seferlik vardiya uygulaması"
- **Sağlık kuruluşlarında kullanılmaya başlanan uygulama** tanımına tam uyuyor. İki taraflı bir pazar: bir tarafta özel hastaneler, bakım/huzurevleri ve evde bakım firmaları, diğer tarafta boş saatlerinde ek iş arayan hemşire, bakıcı, ATT ve sağlık teknikerleri.
- Reklam mesajı basit ve viral: *"Bakım çalışanıysan bu uygulamayı kullanmalısın: yan işle ayda 50 bin yen."* Hepsi son bir ayda açılmış 57 reklamla yoğun bir kampanya yürütüyor.
- **Uyarlama:** Türkiye'de özel sağlık kuruluşlarında ve bakım merkezlerinde personel açığı ve sirkülasyon yüksek. Gelir modeli: kurumdan vardiya başına komisyon.
- **Dikkat:** Kamu hastanelerinde çalışan sağlık personelinin dışarıda ek iş yapması mevzuatla sınırlı. Hedef kitleyi özel sektör çalışanları, bakım personeli ve yeni mezunlar olarak tutun. İş hukuku ve SGK tarafında danışmanlık alın.

### 2. Boomcare / Dadadoc → "çocuk ateşi için akıllı termometre + gece uzaktan çocuk doktoru"
- **Hasta yakını** (ebeveyn) odaklı. Reklam mesajı güçlü bir duygusal anı yakalıyor: *"Çocuğu zar zor uyuttun, şimdi hastaneye mi gideceksin? Uyandırma, yanında muayene ol."*
- Donanım (termometre) ile uygulamanın birlikte satılması sadakat yaratıyor ve kopyalanmasını zorlaştırıyor. Şirket Ocak 2026'da yatırım aldı ve Eylül'de reklamlarını hızla artırmaya başladı.
- **Uyarlama:** Türkiye'de gece çocuk acillerinin yoğunluğu biliniyor. Akıllı termometre + ateş takibi + gerektiğinde çocuk doktoruyla görüntülü görüşme. Uzaktan muayene, ilk rapordaki gibi Sağlık Bakanlığı uzaktan sağlık hizmetleri izni gerektirir. Termometre tarafı ise tıbbi cihaz mevzuatına (TİTCK) tabi.

### Bonus: Modoodoc / My Doctor modeli
Kore'de en uzun süre açık kalan reklamlar fiyat karşılaştırma ve şeffaflık vaadine dayanıyor ("lazer, diş tedavisi, ilaç için en ucuz yer"). Türkiye'de özel klinik, diş ve estetik fiyatlarının şeffaf olmadığı düşünülürse "klinik fiyat karşılaştırma + yorum + randevu" uygulaması da güçlü bir aday.

## İlk raporla birlikte genel tablo

| Bölge | Kazanan model | Örnek |
|---|---|---|
| ABD | AI ön-muayene + ucuz video muayene | Doctronic |
| Brezilya | Abonelik gerektirmeyen ucuz anlık tele-muayene | Doutor Benefícios, Doutor Social |
| Kore | Uzaktan muayene + fiyat karşılaştırma; çocuk odaklı tele-muayene | My Doctor, Modoodoc, Boomcare |
| Japonya | Sağlık personeli için vardiya pazaryeri; sağlık kaydı uygulaması | Kaitech, Pasha-tto Karte |

**Ortak sinyal:** Dört ülkede de büyüyen uygulamalar reklamlarının çoğunu marka hesabından değil, **influencer ve gerçek kullanıcı hesaplarından** yayınlıyor ve kişiye özel indirim kodu kullanıyor.

## Sınırlamalar
- Bütçe nedeniyle her aramada yalnızca 30 reklam çekildi. "Bakım uygulaması" aramasında Kaitech baskın çıktı; daha geniş bir taramada başka adaylar da bulunabilir.
- Meta bu ülkelerdeki ticari reklamlar için harcama ve gösterim verisi vermiyor. Değerlendirme, reklamların ne kadar süre açık kaldığına ve yeni reklam açılma hızına dayanıyor.
- Apify faturası reklam başı ücretin yanında platform kullanım bedeli de içeriyor. Kalan yaklaşık $0,7 ek bir tarama için yeterli değil.

## Kaynaklar
- [Kaitech – 3 yıl üst üste 1 numara (PR Times)](https://prtimes.jp/main/html/rd/p/000000044.000043426.html)
- [Kaitech kurumsal sayfa](https://caitech.co.jp/lp/office/)
- [My Doctor – resmi site](https://my-doctor.io/)
- [My Doctor – uzaktan muayene yasalaştıktan sonra (Nate News)](https://news.nate.com/view/20260126n01127)
- [Dadadoc Healthcare yatırım haberi (Money Today)](https://www.mt.co.kr/future/2026/01/21/2026012115583851712)
- [Boomcare – App Store](https://apps.apple.com/kr/app/%EB%B6%90%EC%BC%80%EC%96%B4-boomcare/id6503333312)
- Meta Reklam Kütüphanesi page_id: Kaitech 963696470154018 / 2302520186660190, Boomcare 377426748777143, Modoodoc 1621578194809405, Pasha-tto Karte 152364211296621, Pillyze 104727362069818
