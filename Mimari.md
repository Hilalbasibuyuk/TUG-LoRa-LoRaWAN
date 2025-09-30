## Soru işaretleri veya durumlar

- Hangi cihazları kullanacağız?
- Cihazların hangi özelliği mimariyi güzel etkiliyor?
- Ödün vermememiz gereken şeyler menzil ve internetli bir kablosuz haberleşme olamaz(internetin olmadığı ortamlarda bu sistemi arayacağız). Ödün verebileceğimiz şey hız olabilir.
- Ek olarak hızın, menzilin artması için cihazlar kullanılabilir.



### Hızı yüksek menzili az olan bir LoRa cihazına, ek cihazlar kullanarak menzili artırmak ve böylece hızın da artmasını sağlamak.

### Hızı az menzili yüksek olan bir lora cihazını kullanmak (ek maliyeti azaltır ama hız da az olur)

### Hem hızı hem de menzili yüksek bir gelişmiş teknolojili Lora'nın yerini alabilecek cihaz bulmak

---

### Teknolojiler

- **LR-FHSS (Long-Range Frequency Hopping Spread Spectrum)**:
LoRaWAN ekosistemine eklenen LR-FHSS modu. Frekans atlaması sayesinde parazitlere karşı çok dayanıklı, ağ kapasitesini artırır ve bazı durumlarda daha iyi pratik menzil/sensitivite sağlar. Özellikle yoğun ortamlarda faydalı.

- **FLRC (Fast Long Range Communication)**
Semtech’in daha yüksek veri hızı hedefleyen “fast” fiziksel katmanı. LoRa’nın hassasiyetine yakın menzil tuttururken veri hızını ciddi şekilde artırıyor (kullanıma göre).

- **2.4 GHz LoRa / SX1280 family (FLRC, LoRa @2.4GHz)**
Semtech’in SX1280 gibi çipleri, 2.4 GHz bandında LoRa/FLRC ve GFSK destekleyerek yüksek veri hızları (LoRa’da teorik tens kbps–200 kbps, FLRC çok daha yüksek) ve farklı çalışma bölgeleri sağlıyor. Ancak 2.4 GHz fiziksel olarak 868 MHz/433 MHz kadar iyi penetrasyon sağlamaz — yani açık alanda LOS varsa hız/menzil dengesi iyi, ama engellerde daha kötü olabilir


- **Semtech “Gen-4 / LoRa Plus**
Semtech’in yeni nesil LR2021/LoRa-Plus serisi hem daha yüksek hızları (FLRC ile Mbps’lere kadar raporlanıyor) hem de daha iyi enerji verimliliğini hedefliyor; çok protokollü, daha yüksek tx gücü opsiyonları ve geliştirilmiş sensivity ile daha uzak mesafe/yüksek throughput kombinasyonlarına izin veriyor. Bu, “klasik LoRa’dan hem daha hızlı hem daha esnek” bir noktaya işaret ediyor





### LoRa'nın yerini alabilecek cihazlar listesi
- **LR2021 (2025 Ekim ayında üretimi planlanıyor)** : Bu çok protokollü alıcı-verici, 2,6 Mbps'ye kadar veri hızlarında LoRa, LoRaWAN® ve Hızlı Uzun Menzilli İletişim (FLRC) ile uyumludur ve
bu da onu yapay zeka destekli IoT çözümleri için uygun hale getirir. Ayrıca, kısa menzilli, düşük güçlü kablosuz protokollerde yaygın olarak kullanılan çeşitli fiziksel katman modülasyonlarını destekleyerek eski cihazlarla uyumluluğu garanti eder.
- **LR2012(2026 2. çeyreğinde üretimi planlanıyor)** : GHz altı işlemlere odaklanan bu cihaz, -142 dBm'ye kadar gelişmiş hassasiyet sunarak geleneksel IoT dağıtımları için idealdir.
- **LR2022(2026 1. çeyreğinde üretimi planlanıyor)** : Çift bantlı bir çözüm olarak tasarlanan bu cihaz, maliyet etkin bir profili korurken küresel alt GHz, 2,4 GHz veya uydu bağlantısı gerektiren uygulamalara hitap ediyor.


### Yüksek Güçlü RF Modülleri LoRa yerine kullanılabilir bu modüllere örnekler
- RFM300P 433/868 MHz 1W/4W RF Modül
- RF4463F30 1W RF Modül
- SV6300 1W RF Modül




### Temel katman (Yerel)

- LoRa / LoRaWAN → Enerji, tarım, akıllı şehir sensörleri.
- ZigBee / Thread / WirelessHART → Fabrika otomasyonu, bina içi sistemler.
- Özel RF modülleri (UHF/VHF) → Savunma, acil durum haberleşmesi.
- MiMO LoRa (Multiple Input Multiple Output)
- NB-Fi (Narrow Band Fidelity)
- DASH7 (Active RFID)
- Sigfox (Global Ağ - Türkiye'de Yok)
- Weightless-P
- Custom UHF/VHF Data Link
- Software Defined Radio (SDR)
- CC1312R - Sub-1 GHz Wireless MCU


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



### Farklı bir alternatif iletişim protokolü: - Yüksek Güçlü RF (Radyo Frekans) Modülleri
- Bu modüller, genellikle lisanssız ISM (Industrial, Scientific, and Medical) bantlarında (örn. 433 MHz, 868 MHz, 915 MHz) çalışır.

- Prensip: LoRa gibi, doğrudan radyo sinyalleri kullanırlar, ancak kendi modülasyon ve protokollerini kullanırlar.

- Avantajı: Uygun yönlü antenler ve yüksek çıkış gücü (yasal sınırlara dikkat ederek) ile 10 km mesafeyi doğrudan Noktadan Noktaya (Point-to-Point) aşma potansiyeli vardır. Veri hızı, LoRa'ya göre biraz daha yüksek olabilir.

- Dezavantajı: Görüş hattı (Line of Sight - LOS) LoRa'dan daha kritiktir. Aradaki en küçük engel bile sinyal kalitesini düşürebilir. Kurulumu, anten ayarlaması ve yasal güç sınırlarına uyumu daha fazla dikkat gerektirebilir.





### Sesli iletişim için
**Amateur/Halk Bandı Radyoları (Lisans/İzin Gerektirebilir)**
- **Prensip:** Amatör Telsizcilik (Ham Radio) cihazları veya yasal sınırlar dahilinde **Lisanssız El Telsizleri (PMR446/FRS)** gibi halk bandı telsizleri kullanılır.
- **Avantajı:** Sesli iletişim kurmak için idealdir. Amatör telsizler, röle istasyonları (bazı yerlerde önceden kurulmuş) kullanarak 10 km'den çok daha öteye erişebilir.
- **Dezavantajı:** **Amatör Telsiz:** Kullanım için resmi lisans (Türkiye'de KEGM tarafından verilen) ve sınav gereklidir. **Halk Bandı (PMR446 vb.):** Güçleri ve menzilleri çok düşüktür (genellikle 1-5 km arası). 10 km mesafeyi ancak çok açık bir alanda, çok güçlü bir antenle ve yüksek bir noktadan aşabilir. **Veri iletişimi (Sayısal İletim)** için özel donanım ve protokol bilgisi (örn. APRS, Packet Radio) gereklidir.





## ! Bluetooth'a gerek kalmayabilir








# KAYNAKÇA
- https://www.semtech.com/company/press/semtech-lora-gen-4-addresses-low-power-wireless-range-and-speed-limitations
- https://nb-fi.org/
