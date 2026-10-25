# AYSPAK TF30 · Safety 4.0 Laboratuvarları

**Yazılım Güncel Konular | Laboratuvar 1–2–3–4**

Tava tipi kutu kurma makinesi üzerinden emniyet fonksiyonları, endüstriyel ağ bölgelemesi, siber riskler ve güvenli uzak erişim incelemesi.

| Teslim bilgisi | Açıklama |
|---|---|
| Hazırlayan | Muhammed Emin Cimen |
| Tarih | 25 Ekim 2026 |
| Makine | AYSPAK-TF30 Tava Tipi Kutu Kurma Makinesi |
| Kapsam | İlk dört laboratuvar; Laboratuvar 5–6–7 kapsam dışıdır |
| Yöntem | Üreticinin açık bilgileri + açıkça belirtilmiş eğitim varsayımları |
| Grup bilgisi | Bireysel çalışma olarak düzenlenmiştir; ders grubu bilgisi paylaşılmamıştır |

## Doldurulmuş föyler

| Laboratuvar | İçerik | Çıktı / Evidence Pack |
|---|---|---|
| [01 · Emniyet mimarisi](laboratuvar-1/README.md) | Sekiz sorunun cevabı ve emniyet fonksiyonu haritası | Safety Function Map · EP 03 |
| [02 · IEC 62443](laboratuvar-2/README.md) | Varlık bölgeleri, bağlantılar ve altı uzak erişim kararı | Zone / Conduit Diagram · EP 05 |
| [03 · Tehdit ve risk](laboratuvar-3/README.md) | Üç fiziksel sonuç senaryosu, puanlama ve öncelikler | Risk Register · EP 04 |
| [04 · Güvenli uzak erişim](laboratuvar-4/README.md) | Başlangıç–hedef şemaları ve bağımsız emniyet gereksinimleri | Secure Architecture · EP 02 + EP 06 |

**Okuma sırası:** [Makine ve varsayımlar](kaynaklar/makine-ve-varsayimlar.md) → Laboratuvar 1 → 2 → 3 → 4.

## İki kaynak föy nasıl kullanıldı?

Dersin **Genel Sürüm** PDF'si şişeleme hattını, **PaketPro 3000 Sürümü** ise örnek paketleme makinesini esas alır. İlk dört laboratuvarın amaçları ve çıktıları ortaktır. Bu depoda genel föyün tüm soruları cevaplanmış, PaketPro sürümündeki makineye özgü yönlendirmeler TF30 bağlamına uyarlanmıştır. Aynı ödev iki kez tekrarlanmamıştır.

PaketPro'da verilen kesme bıçağı, ışık perdesi, açık bakım modülü ve varsayılan parola bilgileri **TF30'a ait bulgu değildir**. Özellikle siber zafiyet senaryoları üretici hakkında bir tespit olarak okunmamalıdır.

## Çalışmanın sınırı

Bu çalışma ders için hazırlanmış bir masa başı değerlendirmesidir. Gerçek makinede inceleme, ağ taraması, duruş süresi ölçümü veya emniyet doğrulaması yapılmamıştır. Şemalar eğitim için önerilen işlevsel ilişkileri gösterir; uygulama projesi, uygunluk belgesi veya doğrulanmış fabrika ağı çizimi değildir. Sayısal risk puanları eğitim değerlendirmesidir; PLr/SIL hesabının yerine geçmez.

Kaynaklar ve doğrulanamayan ayrıntılar [makine dosyasında](kaynaklar/makine-ve-varsayimlar.md) açıklanmıştır. Şemalar GitHub'ın Mermaid görüntüleyicisiyle okunabilir.
