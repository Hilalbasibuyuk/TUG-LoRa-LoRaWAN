## Soru işaretleri veya durumlar

- Hangi cihazları kullanacağız?
- Cihazların hangi özelliği mimariyi güzel etkiliyor?
- Ödün vermememiz gereken şeyler menzil ve internetli bir kablosuz haberleşme olamaz(internetin olmadığı ortamlarda bu sistemi arayacağız). Ödün verebileceğimiz şey hız olabilir.
- Ek olarak hızın, menzilin artması için cihazlar kullanılabilir.



### Hızı yüksek menzili az olan bir LoRa cihazına, ek cihazlar kullanarak menzili artırmak ve böylece hızın da artmasını sağlamak.

### Hızı az menzili yüksek olan bir lora cihazını kullanmak (ek maliyeti azaltır ama hız da az olur)

### Hem hızı hem de menzili yüksek bir gelişmiş teknolojili Lora'nın yerini alabilecek cihaz bulmak

---

### LoRa'nın yerini alabilecek cihazlar listesi
- **LR2021 (2025 Ekim ayında üretimi planlanıyor)** : Bu çok protokollü alıcı-verici, 2,6 Mbps'ye kadar veri hızlarında LoRa, LoRaWAN® ve Hızlı Uzun Menzilli İletişim (FLRC) ile uyumludur ve
bu da onu yapay zeka destekli IoT çözümleri için uygun hale getirir. Ayrıca, kısa menzilli, düşük güçlü kablosuz protokollerde yaygın olarak kullanılan çeşitli fiziksel katman modülasyonlarını destekleyerek eski cihazlarla uyumluluğu garanti eder.
- **LR2012(2026 2. çeyreğinde üretimi planlanıyor)** : GHz altı işlemlere odaklanan bu cihaz, -142 dBm'ye kadar gelişmiş hassasiyet sunarak geleneksel IoT dağıtımları için idealdir.
- **LR2022(2026 1. çeyreğinde üretimi planlanıyor)** : Çift bantlı bir çözüm olarak tasarlanan bu cihaz, maliyet etkin bir profili korurken küresel alt GHz, 2,4 GHz veya uydu bağlantısı gerektiren uygulamalara hitap ediyor.


### Temel katman (Yerel)

- LoRa / LoRaWAN → Enerji, tarım, akıllı şehir sensörleri.
- ZigBee / Thread / WirelessHART → Fabrika otomasyonu, bina içi sistemler.
- Özel RF modülleri (UHF/VHF) → Savunma, acil durum haberleşmesi.


### Ağ Genişletme Katmanı (Mesh / Repeater / Gateway)
- Tek cihazın kapsama alanı yetmediğinde mesh ağ yapısı kuruluyor.

- Tekrarlayıcı (repeater) veya yönlendirici (router) cihazlar ekleniyor.

- Gateway cihazları: Yerel ağdaki veriyi toplayıp gerektiğinde internete veya uyduya çıkarıyor.

**Örneğin:** Bir petrol sahasında her sensör internete bağlanmaz. Sensörler LoRa ile birbirine, oradan bir LoRaWAN Gateway’e; gateway de uyduya veya merkeze bağlanır.



 ### Yedek / Global İletişim Katmanı

- Kurumsal çözümler genelde yedekli haberleşme ister. Bunun için:

- Uydu modemleri (Iridium, Inmarsat, Swarm, Starlink IoT) kullanılır.

- Çift ağ stratejisi: Hem LoRa hem uydu, hem ZigBee hem LTE gibi.

- Özel güvenli ağ protokolleri (VPN, şifreleme, askeri frekans atlamalı sistemler).

Böylece internet olmasa bile cihazlar birbirleriyle haberleşir, kritik veriler gerektiğinde uyduyla merkeze aktarılır.






### Kurumsal Stratejiler

- Enerji şirketleri (petrol, doğalgaz, elektrik şebekesi) → LoRaWAN + Uydu yedekleme.

- Savunma / güvenlik → Özel RF sistemleri + Mesh + Uydu.

- Tarım / akıllı şehir → LoRaWAN / Sigfox + GSM fallback (opsiyonel).

- Ulaşım / lojistik → GSM kapsaması varsa LTE/5G, yoksa uydu tabanlı IoT modemler.

