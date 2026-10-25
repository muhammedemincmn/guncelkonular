# Laboratuvar 3 · Threat & Risk + Risk Matrix

**Çıktı:** Risk Register · **EP 04 — Risk Assessment**

**Makine:** AYSPAK-TF30 · **Hazırlayan:** Muhammed Emin Cimen · **Tarih:** 25.10.2026

[← Ana sayfa](../README.md) · [Önceki](../laboratuvar-2/README.md) · [Sonraki →](../laboratuvar-4/README.md)

> Bu kayıtlar V1–V4 ve V6 eğitim senaryolarının, hedef önlemler uygulanmadan önceki değerlendirmesidir. Gerçek TF30'da saldırı, açıklık veya yaralanma gözlemlenmemiştir. Fiziksel sonuca ulaşmak için gereken emniyet başarısızlığı her senaryoda ayrıca belirtilmiştir.

## Puanlama yöntemi

Föydeki **Skor = L × S × E** yöntemi kullanılmıştır; her çarpan 1–3 arasındadır. Föy, çarpanların ayrıntılı ölçeğini vermediğinden aşağıdaki çalışma tanımları benimsenmiştir.

| Değer | L — Senaryonun gerçekleşme olasılığı | S — Yaralanma şiddeti | E — İnsanın tehlikeye maruziyeti |
|---|---|---|---|
| 1 | Birden fazla özel koşul gerektirir; düşük | İlk yardımla giderilebilir hafif zarar | Seyrek, kısa bakım müdahalesi |
| 2 | Belirli koşullarda mümkün; orta | Tıbbi müdahale gerektiren ciddi, geri döndürülebilir zarar | Aralıklı temizlik / ayar müdahalesi |
| 3 | Varsayılan zayıf başlangıç koşullarında yüksek | Kalıcı hasar, uzuv kaybı veya ölüm potansiyeli | Sık veya uzun süreli tehlikeli bölge erişimi |

Bunlar ölçülmüş sıklıklar değildir. L tüm olay zinciri için öznel eğitim tahminidir; E insanın maruziyetini temsil eder. Kategoriler föyden alınmıştır: **18–27 Kritik · 9–17 Yüksek · 4–8 Orta · 1–3 Düşük**. Ayrıca **S=3 olan senaryo puanı düşük olsa da öncelikli ele alınır**. Bu istisna sayısal puanı değiştirmez.

## Üç senaryo ve risk kaydı

| ID | Kim → giriş kapısı → eylem → zincir → fiziksel sonuç | L | S | E | Skor | Sayısal bant | İşlem önceliği |
|---|---|---:|---:|---:|---:|---|---|
| R1 | Dış saldırgan → V4'teki doğrudan bakım erişimi ve ortak hesap → üretim programını ve erişilebildiği varsayılan emniyet ayarını değiştirir → kapak açıkken duruş engeli yetersiz kalır, operatör karton sıkışmasını giderirken kafa hareket eder → el/parmak ezilmesi, kalıcı hasar | 2 | 3 | 3 | **18** | Kritik | **1 · Kritik** |
| R2 | Ele geçirilmiş servis bilgisayarı → yetkili görünen bakım oturumu → tutkal sıcaklık ayarı yükseltilir → ayrıca bağımsız sıcaklık sınırlandırması yoksa / başarısızsa tehlikeli ısınma oluşur → temizlikte sıcak tutkal teması, ciddi yanık | 2 | 2 | 3 | **12** | Yüksek | **3 · Yüksek** |
| R3 | Yetkisiz / hatalı işlem yapan bakım personeli → kontrolsüz USB ve yerel mühendislik istasyonu → eski, doğrulanmamış programı geri yükler → yeniden başlatma kilidi hatalı olur ve bakımda enerji izolasyonu uygulanmamıştır → enerji geri gelince kafa beklenmedik hareket eder, bakım personeli ağır şekilde sıkışır | 1 | 3 | 1 | **3** | Düşük | **2 · S=3 nedeniyle yükseltilmiş** |

R1'de uzaktan erişim tek başına emniyet fonksiyonunu bozulmuş saydırmaz: emniyet değişikliği yetkisinin de ele geçirilmesi veya korumanın yetersizliği gerekir. R2'de yalnız reçete değişikliği, bağımsız sıcaklık sınırlandırması sağlıklıysa tanımlanan zinciri tamamlamaz. R3'te program hatası ile bakım izolasyonu eksikliği birlikte varsayılmıştır. Saldırı yolu kapanır veya bu bağımsız korumalar doğrulanırsa olasılık yeniden değerlendirilir.

## Her risk için karşılık ve gerekli kanıt

| ID | Riski azaltacak gereksinimler | Doğrulama için gerekli kanıt |
|---|---|---|
| R1 | Doğrudan dış erişim kaldırılmalı; MFA ve kişisel hesap olmalı; uzaktan üretim yetkisi emniyet programına ulaşmamalı; kapak açıkken tehlikeli hareket engellenmeli. | Erişim kural incelemesi, rol matrisi, emniyet değişiklik kaydı ve kontrollü kapak/duruş doğrulama tutanağı |
| R2 | Sıcaklık yazma yetkisi sınırlandırılmalı; limitler doğrulanmalı; proses kontrolünden bağımsız aşırı sıcaklık tepkisi ve erişim koruması sağlanmalı. | Onaylı limit listesi, sıcaklık koruması işlev doğrulaması, kalibrasyon ve değişiklik kaydı |
| R3 | USB ve yazılım yükleme yetkilendirilmeli; yalnız doğrulanmış sürüm geri yüklenmeli; bakımda enerji izolasyonu yapılmalı; enerji dönüşü otomatik start yaratmamalı. | Yedek sürüm/bütünlük kaydı, bakım izolasyonu tutanağı ve kontrollü enerji dönüşü doğrulaması |

Bunlar yapılması gereken doğrulamalardır; bu çalışmada test sonucu veya artık risk puanı üretilmemiştir. Önlemler uygulanmadan riskin düştüğü iddia edilemez.

## 1. En yüksek öncelikli senaryo hangisi, neden?

**R1:** Hem 18 ile kritik banttadır hem de sık müdahale edilen biçimlendirme bölgesinde kalıcı el/parmak hasarı potansiyeli taşır; bu nedenle ilk ele alınacak senaryodur.

## 2. S=3 olup skoru düşük kalan senaryo var mı?

**R3'ün puanı 1 × 3 × 1 = 3'tür.** Sayısal bandı düşük olsa da kalıcı zarar potansiyeli nedeniyle ayrı bir **S=3 işareti** ve ikinci işlem sırası verilmiştir. Böylece seyrek bakım olayı tablonun sonunda kaybolmaz. R2 yüksek puanlı olsa da bu çalışmada S=3 senaryolarından sonra ele alınmıştır; gerçek tesiste aksiyonlar eşzamanlı yürütülebilir.
