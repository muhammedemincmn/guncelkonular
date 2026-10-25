# Makine, kanıt sınırı ve ortak varsayımlar

[← Ana sayfa](../README.md)

## Üretici bilgisi · K1

Seçilen makine **AYSPAK-TF30 Tava Tipi Kutu Kurma Makinesi**dir. Üreticinin açıklamasında personelin magazini doldurması, kartonun konveyöre alınması, biçimlendirme kafasının aşağı hareketi, kartonun kıvrılması ve tutkallanması anlatılır. Sayfa servo teknolojisini, PLC dokunmatik panelini ve sıcak tutkal istasyonunu belirtir. Bu mekanik süreç bütün laboratuvarların ortak temelidir. [AYSPAK ürün sayfası](https://www.ayspak.com.tr/tr/u/kutulama-makinalari/kutu-yapma-tava-tipi-makinesi)

Sayfanın tanıtımında ve genel özelliklerinde 40 kutu/dakikaya kadar kapasite yazarken teknik tabloda 6–12 adet/dakika değerleri bulunur. Bu tutarsızlık çözümlenmeden kesin kapasite kabul edilmemiştir; risk puanları kapasite üzerinden hesaplanmamıştır. [K1]

## Eğitim varsayımları · V

| Kod | Ortak kabul | Kanıt durumu |
|---|---|---|
| V1 | Sıkışma giderme sırasında operatör tehlikeli bölgeye erişebilir. | Görev senaryosu; saha gözlemi yoktur. |
| V2 | Hedef mimaride acil durdurma, izlenen kapak kilidi, ayrı emniyet mantığı ve güvenli çıkış elemanları bulunacaktır. | Önerilen gereksinimlerdir; mevcut donanım doğrulanmamıştır. |
| V3 | İnceleme için sürücüler, mühendislik bilgisayarı ve bir servis erişim yolu modellenmiştir. | Marka, protokol ve gerçek bağlantı bilinmemektedir. |
| V4 | Başlangıç senaryosunda doğrudan uzak erişim, ortak hesap ve kontrolsüz USB kullanımı varsayılmıştır. | Yalnızca eğitim senaryosudur; AYSPAK'ta mevcut zafiyet iddiası değildir. |
| V5 | Hedefte DMZ, erişim ağ geçidi, jump server ve bağımsız emniyet bölgesi önerilmiştir. | Kurulum yapılmamıştır. |
| V6 | Sıcak tutkal ünitesinde kontrol edilebilir bir ısıtma düzeni olduğu modellenmiştir. | Isıtıcı devresi ve bağımsız sıcaklık koruması doğrulanmamıştır. |

Safety PLC, ışık perdesi, STO, emniyet freni, güvenli pnömatik valf, SCADA, bulut, Wi-Fi ve robotun mevcut olduğu doğrulanmamıştır. Robot, SCADA, bulut ve Wi-Fi bu TF30 senaryosuna eklenmemiştir. Işık perdesi yerine örnek erişim koruması olarak izlenen kapak ele alınmıştır; bu da V2 kapsamında öneridir.

## Kaynaklar

- **K1 — Makine:** [AYSPAK-TF30 resmî ürün sayfası](https://www.ayspak.com.tr/tr/u/kutulama-makinalari/kutu-yapma-tava-tipi-makinesi), erişim: 25.10.2026.
- **K2 — Ders föyü:** INSPECCO × KRIPTARIUM, *Safety 4.0 Bootcamp — Laboratuvar Föyleri, Genel Sürüm*, kullanıcı tarafından sağlanan `2.1. lab_foyleri_genel.pdf`, s. 2–5.
- **K3 — Ders föyü:** INSPECCO × KRIPTARIUM, *Safety 4.0 Bootcamp — Laboratuvar Föyleri, PaketPro 3000 Sürümü*, kullanıcı tarafından sağlanan `2.2 lab_foyleri_paketpro.pdf`, s. 2–5.
- **K4 — OT güvenliği:** [NIST SP 800-82 Rev. 3](https://csrc.nist.gov/pubs/sp/800/82/r3/final), özellikle ağ bölümleme ve uzak erişim yaklaşımı. Rev. 3 bu çalışmada kullanılan yayımlanmış sürümdür.
- **K5 — Bölgeler ve bağlantılar:** [IEC'nin IEC 62443 özeti](https://syc-se.iec.ch/deliveries/cybersecurity-guidelines/security-standards-and-best-practices/iec-62443/). Bölgeleme yaklaşımı kullanılmış; madde bazında uygunluk veya SL sertifikasyonu iddia edilmemiştir.
- **K6 — Güvenli duruş:** [Pilz, Safe motion with PMCprotego S](https://www.pilz.com/en-INT/products/drive-technology/servo-amplifiers/pmcprotego-safe-motion). STO ile kontrollü duruşun farklılığı için teknik referanstır; TF30'un Pilz kullandığı anlamına gelmez.
- **K7 — Düşey eksen:** [Siemens, Hanging loads with SIMATIC Axis and SINAMICS](https://cache.industry.siemens.com/dl/files/260/109807260/att_1104659/v1/109807260_HangingAxis_DOC_v11_en.pdf), §2.4. TF30'un Siemens kullandığı anlamına gelmez.

## Gerçek uygulama öncesi gereken kanıtlar

Elektrik/pnömatik şemalar, kontrol ve sürücü modelleri, emniyet bileşeni belgeleri, erişim mesafeleri, en kötü duruş süresi, düşey mekanizmanın yük tutma düzeni, sıcaklık limitleri, gerçek ağ envanteri ve yetkilendirme kayıtları gerekir. Bunlar paylaşılmadığından bu çalışmada ölçülmüş değer veya kesin PLr/SIL seviyesi verilmemiştir.
