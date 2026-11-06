# AYSPAK TF30 · Safety 4.0 Laboratuvarları

**Yazılım Güncel Konular | Laboratuvar 1–2–3–4–5–6–7**

Tava tipi kutu kurma makinesi üzerinden emniyet fonksiyonları, endüstriyel ağ bölgelemesi, siber riskler, güvenli uzak erişim, yama yönetimi, olay müdahalesi ve yapay zekâ kararları incelemesi.

| Teslim bilgisi | Açıklama |
|---|---|
| Hazırlayan | Emin Çimen |
| Öğrenci numarası | 235541088 |
| İlk teslim / güncelleme | 25 Ekim 2026 / 6 Kasım 2026 |
| Makine | AYSPAK-TF30 Tava Tipi Kutu Kurma Makinesi |
| Kapsam | Laboratuvar 1–7; ilk dört sayfa korunmuş, 5–6–7 eklenmiştir |
| Yöntem | Üreticinin açık bilgileri + açıkça belirtilmiş eğitim varsayımları |
| Grup bilgisi | Bireysel çalışma olarak düzenlenmiştir; ders grubu bilgisi paylaşılmamıştır |

## PDF teslim dosyaları

**[Yedi laboratuvarın doldurulmuş birleşik PDF’sini aç / indir](Tümü.pdf)**

PaketPro 3000 kaynak PDF’sinin **Laboratuvar 1–2–3–4–5–6–7 sayfaları**, orijinal metinleri ve tasarımı değiştirilmeden doldurulmuştur. Cevaplar özellikle **AYSPAK-TF30** makinesi için yazılmıştır. Her laboratuvar klasöründe ilgili tek sayfalık PDF ve önizlemesi bulunur. Kaynaktaki 2/8–8/8 sayfa numaraları korunmuştur; birleşik teslim dosyası yedi sayfadır. İlk dört laboratuvarın 25.10.2026 tarihli sayfaları aynen korunmuş; yeni üç sayfa 06.11.2026 tarihiyle doldurulmuştur.

PDF’deki PaketPro senaryo metinleri kaynak föye aittir; TF30 hakkında doğrulanmış bulgu sayılmaz. Bu ayrım cevaplarda belirtilmiştir.

## Doldurulmuş föyler

| Laboratuvar | İçerik | Çıktı / Evidence Pack |
|---|---|---|
| [01 · Emniyet mimarisi](laboratuvar-1/README.md) | Sekiz sorunun cevabı ve emniyet fonksiyonu haritası | Safety Function Map · EP 03 |
| [02 · IEC 62443](laboratuvar-2/README.md) | Varlık bölgeleri, bağlantılar ve altı uzak erişim kararı | Zone / Conduit Diagram · EP 05 |
| [03 · Tehdit ve risk](laboratuvar-3/README.md) | Üç fiziksel sonuç senaryosu, puanlama ve öncelikler | Risk Register · EP 04 |
| [04 · Güvenli uzak erişim](laboratuvar-4/README.md) | Başlangıç–hedef şemaları ve bağımsız emniyet gereksinimleri | Secure Architecture · EP 02 + EP 06 |
| [05 · SBOM / CVE / Yama](laboratuvar-5/README.md) | Etkilenebilirlik, yama/test kararı ve telafi edici önlemler | Vulnerability Decision · EP 09 · 10 · 11 |
| [06 · Olay müdahalesi](laboratuvar-6/README.md) | İlk müdahale, kanıt koruma, bildirim ve güvenli geri dönüş | Incident Workflow · EP 13 |
| [07 · Yapay zekâ ve emniyet](laboratuvar-7/README.md) | Yanlış sınıflandırma, bozuk girdi ve düşük güven kararları | AI Fail-Safe Decision · EP 03 + EP 15 |

**Okuma sırası:** [Makine ve varsayımlar](kaynaklar/makine-ve-varsayimlar.md) → Laboratuvar 1 → 2 → 3 → 4 → 5 → 6 → 7.

## İki kaynak föy nasıl kullanıldı?

Dersin **Genel Sürüm** PDF'si şişeleme hattını, **PaketPro 3000 Sürümü** ise örnek paketleme makinesini esas alır. Yedi laboratuvarın ortak soru ve çıktıları TF30 bağlamında cevaplanmıştır. PaketPro sürümündeki makineye özgü yönlendirmeler, cevaplarda TF30 için belirtilen varsayımlarla ele alınmıştır. Aynı ödev iki kez tekrarlanmamıştır.

PaketPro'da verilen kesme bıçağı, ışık perdesi, açık bakım modülü ve varsayılan parola bilgileri **TF30'a ait bulgu değildir**. Özellikle siber zafiyet senaryoları üretici hakkında bir tespit olarak okunmamalıdır.

## Çalışmanın sınırı

Bu çalışma ders için hazırlanmış bir masa başı değerlendirmesidir. Gerçek makinede inceleme, ağ taraması, duruş süresi ölçümü veya emniyet doğrulaması yapılmamıştır. Şemalar eğitim için önerilen işlevsel ilişkileri gösterir; uygulama projesi, uygunluk belgesi veya doğrulanmış fabrika ağı çizimi değildir. Sayısal risk puanları eğitim değerlendirmesidir; PLr/SIL hesabının yerine geçmez.

Kaynaklar ve doğrulanamayan ayrıntılar [makine dosyasında](kaynaklar/makine-ve-varsayimlar.md) açıklanmıştır. Şemalar GitHub'ın Mermaid görüntüleyicisiyle okunabilir.
