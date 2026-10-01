# Sağlık Alanında Yükselen Uygulamalar — Instagram Reklam Analizi (ABD + Brezilya)

**Tarih:** 1 Ekim 2026 · **Kaynak:** Meta Reklam Kütüphanesi (Instagram + Facebook), Apify `apify/facebook-ads-scraper` ile çekildi · **Harcama:** ≈ $3,22 / $5
**Ham veri:** `ham_reklam_verisi.csv` (538 reklam)

## Yöntem

1. **Tarama:** Instagram'da şu an yayında olan reklamlar anahtar kelimeyle arandı:
   ABD: `health app`, `caregiver app`, `telehealth app` · Brezilya: `app de saúde`, `aplicativo médico` (her biri 70 reklam).
2. **Eleme:** Sağlık dışı (drama/oyun uygulamaları, hukuk, kozmetik) ve köklü markalar (Flo, Noom, WHOOP, Walgreens) çıkarıldı. Kalanlar arasında **yeni** olan ve **hasta / doktor / hasta yakını / hastane** kullanımına uyanlar seçildi.
3. **Derin analiz:** 8 aday markanın sayfa bazında **toplam reklam sayısı**, **aktif reklam sayısı**, **ilk reklam tarihi** ve **kapanan reklamların süresi** çekildi.

> **Yorum kuralı:** Bir reklam aylardır açıksa marka o reklamdan para kazanıyor demektir (zarar eden reklam birkaç günde kapatılır). Aktif/toplam oranı yüksek ve yeni reklamlar hızla ekleniyorsa marka **ölçekleniyor** demektir.

## Sonuç tablosu

| Uygulama | Ülke | Kim kullanıyor | Toplam reklam | Aktif | İlk reklam | Reklam davranışı |
|---|---|---|---|---|---|---|
| **Doctronic** (AI doktor + $39 video muayene) | ABD | Hasta | **173** | **171** | Mart 2026 (test) | Mart/Nisan'da 2 test reklamı 5–6 günde kapatıldı. **25 Ağu'dan itibaren patlama:** 16 Eyl'de 33, 29 Eyl'de 19 yeni reklam. Kapanan reklam yok. |
| **Doutor Benefícios** (R$49,90 tele-muayene) | BR | Hasta | 34 | **34** | 15 May 2026 | Mayıs'ta açılan reklamlar **~139 gündür hâlâ açık** → kârlı. Reklamda "400 bin kullanıcı" diyor. |
| **Doutor Social** (R$29,90 → R$25, 7/24 doktor) | BR | Hasta | 28 | **28** | 15 Tem 2026 | Tüm reklamlar ~78 gündür açık, hiç kapatılmamış. Aynı modelin ucuz rakibi. |
| **Citizen Health – "Ari"** (nadir hastalıklar için AI asistan) | ABD | **Hasta yakını / bakıcı** | 22 | 21 | 19 May 2026 (test) | Mayıs'taki test reklamı 2 günde kapandı; **13 Ağu'dan beri** açılan reklamların hepsi açık (en eskisi 49 gün). Reklamlar gerçek ebeveynlerin hesaplarından (creator ads). |
| **Commure Scribe** (doktorlar için AI not tutucu) | ABD | **Doktor / klinik** | 37 | 35 | Nis 2025 | Temmuz 2026'dan beri yeniden ölçekleniyor. |
| **Paid.care** (aile bakıcısına maaş) | ABD | Hasta yakını | 12 | 11 | May 2026 | Haziran'dan beri açık reklamlar var. |
| **Caring Village** (bakım koordinasyon uygulaması) | ABD | Hasta yakını + bakım kurumu | 14 | 14 | 8 Eyl 2026 | Çok yeni; henüz test aşamasında. |
| Nourish (diyetisyen, sigorta kapsamlı) | ABD | Hasta | 340 | 302 | Nis 2026 | Büyük ama artık "yeni" değil — referans olarak. |

## 1. Öneri: Doctronic → Türkiye için "AI ön-muayene + ucuz video doktor"

**Neden en güçlü aday:**
- **Yeni ve şu an patlıyor:** 173 reklamın 171'i aktif, neredeyse hepsi son 40 günde açıldı. Bu, testleri bitirip kazanan formülü bulmuş ve bütçeyi hızla artıran bir markanın klasik görüntüsü.
- **Viral reklam formatı:** Reklamların çoğu marka sayfasından değil, onlarca farklı **UGC/influencer hesabından** (Cal, Jhiggsyo, yothatsliz, christinadecarlo…) yayınlanıyor. Örnek metin: *"semptomlarımı yazdım, dakikalar içinde cevap aldım, $39'a video görüşme yaptım, reçeteyi aynı gün aldım — CALLI20 koduyla %20 indirim"*. Kişiye özel indirim kodları = performans ödemeli influencer modeli.
- **Kanıtlanmış büyüme:** Mart 2026'da 40 milyon $ Series B; 1 milyondan fazla kullanıcı, haftalık 300 bin ziyaretçi, 6 ayda 15 kat gelir artışı (STAT News, HLTH).
- **Modelin Latin Amerika'da da çalıştığının kanıtı:** Brezilya'da Doutor Benefícios (139 gündür açık reklamlar, 400 bin kullanıcı) ve Doutor Social aynı vaadi ("hasta olunca evden, saniyeler içinde, ucuza doktor") başarıyla satıyor.

**Türkiye uyarlaması:**
- Ücretsiz AI semptom sohbeti → gerekirse **99–149 TL'lik** anlık video muayene (Brezilya fiyat noktasına benzer).
- Reklam açısı: "Sırf doktora gitmek için izin alma / işten kalma" (Doutor Benefícios'un ana mesajı), çocuk ateşi gece yarısı, yeşil reçete gerektirmeyen ilaçlar.
- Reklam kanalı: Doctronic gibi mikro-influencer + kişiye özel indirim kodu.
- **Mevzuat uyarısı:** Türkiye'de uzaktan sağlık hizmeti Sağlık Bakanlığı'nın *Uzaktan Sağlık Hizmetlerinin Sunumu Hakkında Yönetmelik* kapsamında izne tabidir; reçete/rapor yetkisi hekimdedir. AI'nın otonom reçete yenilemesi (Doctronic'in ABD'de Utah özelinde yaptığı) Türkiye'de mümkün değildir — AI'yı yalnızca triyaj/ön bilgi katmanı olarak konumlayın ve hukuki danışmanlık alın.

## 2. Öneri (daha az rekabetli niş): Citizen Health "Ari" → hasta yakınları için AI bakım asistanı

- Hedef kitle tam olarak **hasta yakınları**: nadir/kronik hastalığı olan çocukların ebeveynleri. Tahlilleri, epikrizleri okuyor, nöbet/ilaç takibi yapıyor, doktora mesaj hazırlıyor, klinik çalışma öneriyor. Aileler için ücretsiz.
- Reklamları gerçek annelerin hesaplarından: *"Oğlumun Angelman sendromu var, nöbetlerle boğuşuyorduk…"* — duygusal, çok paylaşılan format.
- Ağustos'tan beri açılan hiçbir reklam kapatılmamış → çalışıyor. Hasta dernekleriyle (Angelman, Rett) ortaklık kurarak büyüyor.
- **Türkiye uyarlaması:** e-Nabız'dan indirilen raporları/tahlilleri anlamlandıran, ilaç/semptom takip eden ve aileyi bilgilendiren asistan. Reçete yazmadığı için regülasyon riski daha düşük; SMA, otizm, epilepsi, Alzheimer hasta dernekleri ile ortaklık kanalı.

## Diğer dikkat çekenler
- **Commure Scribe** — doktor muayenesini dinleyip notu otomatik yazan AI. Hastane/klinik tarafı için B2B fırsatı (Türkçe tıbbi dikte + HBYS entegrasyonu).
- **Paid.care / Caring Village** — evde bakım yapan aile üyesine yönelik; Türkiye'de "evde bakım maaşı" başvuru ve takip asistanı olarak uyarlanabilir.

## Sınırlamalar
- Meta Reklam Kütüphanesi ABD/Brezilya ticari reklamlarında **harcama ve gösterim verisi vermez**; "kazanıyor" yorumu reklamların açık kalma süresine dayanır.
- Bütçe nedeniyle Meksika/Arjantin taraması yapılmadı (Apify ücretsiz planda eşzamanlı çalıştırma sınırı).
- Anahtar kelime aramaları her sorgu için 70 reklamla sınırlı; farklı kelimelerle başka adaylar çıkabilir.

## Kaynaklar
- [STAT News – Doctronic $40M](https://www.statnews.com/2026/03/23/ai-doctor-startup-doctronic-raises-40-million/)
- [HLTH – Doctronic $40M](https://hlth.com/insights/news/ai-doctor-startup-doctronic-garners-40m-2026-03-24)
- [CNBC – Citizen Health](https://www.cnbc.com/2026/04/11/citizen-health-rare-disease-treatment-ai.html)
- [Fierce Healthcare – Citizen Health & Angelman Foundation](https://www.fiercehealthcare.com/ai-and-machine-learning/rare-disease-foundation-partners-citizen-health-embed-ai-agent-everyday)
- [IRSF – Citizen Health Ari](https://www.rettsyndrome.org/citizenhealth_09-26/)
- Meta Reklam Kütüphanesi: Doctronic page_id 428312257036400, Citizen Health 298139186725904, Doutor Social 908970792304895, Doutor Benefícios 119356663233742
