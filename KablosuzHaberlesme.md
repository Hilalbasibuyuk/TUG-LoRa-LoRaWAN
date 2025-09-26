# Kablosuz Haberleşme

Kablosuz haberleşme, adından da anlaşıldığı gibi veri iletiminin herhangi bir kablo olmadan gerçekleştirilmesine verilen addır. Genellikle veri transferi için radyo dalgaları kullanılır. Genellikle dememin sebebi, kızılötesi gibi radyo dalgaları yerine ışık kullanan teknolojilerin halen hayatımızda olmasından dolayıdır. Evimizde kullandığımız televizyon gibi cihazların uzaktan kumandaları kızılötesi ışık ile haberleşme yapar. Hatta hatırlayacak olursak 2000’li yıllarda kullandığımız cep telefonları, bluetooth yerine kızılötesi haberleşme ile dosya transferi dahi yapabilmekteydi.



Kablosuz cihazlara örnek olarak cep telefonları, GPS cihazları, otopark bariyerlerini açmada kullandığımız kumandalar, otobüslerde bilet olarak kullandığımız kartlar gibi cihazlar verilebilir. Dikkat ettiyseniz bu cihazların bir kısmı sadece alıcı, bir kısmı sadece verici ve bazıları da hem alıcı hem verici olarak görev yapmaktadır. Neredeyse tamamı farklı haberleşme protokolleri kullanır. Bu haberleşme sistemlerinden WiFi, Bluetooth ve NFC gibi bazılarını kendi yaptığımız projelerimizde de kullanabilmekteyiz.



### Kablosuz Haberleşmenin Temel Prensipleri
Kablosuz haberleşmenin temel prensipleri, elektromanyetik dalgaların kullanımı ve bu dalgaların yayılımı üzerine kuruludur. İşte bu prensiplerin ana başlıkları:

- **Elektromanyetik Dalgalar**: Kablosuz haberleşmede, bilgi elektromanyetik dalgalar aracılığıyla iletilir. Bu dalgalar radyo frekansları (RF), mikrodalgalar, kızılötesi ışınlar veya ışık dalgaları olabilir.
- **Modülasyon**: Bilgilerin elektromanyetik dalgalarla iletilebilmesi için taşıyıcı dalga üzerine bindirilmesi gerekir. Bu süreç modülasyon olarak adlandırılır. Başlıca modülasyon teknikleri arasında genlik modülasyonu (AM), frekans modülasyonu (FM) ve faz modülasyonu (PM) bulunur.
- **Frekans Spektrumu**: Kablosuz iletişimde farklı frekans bantları kullanılır. Frekans spektrumu, belirli bir frekans aralığında bilgi iletimi için ayrılmış bantlardan oluşur. Her bir teknoloji veya hizmet belirli frekans bantları kullanır (örneğin, Wi-Fi 2.4 GHz ve 5 GHz bandında çalışır).
- **Antenler**: Elektromanyetik dalgaların iletimi ve alımı için antenler kullanılır. Antenler, elektromanyetik enerjiyi yaymak ve almak için tasarlanmış cihazlardır. Anten tasarımı ve yerleşimi, sinyalin etkin bir şekilde iletilmesi için kritiktir.
- **Yayılım ve Kırılma**: Elektromanyetik dalgalar, serbest uzayda düz bir çizgide yayılır ancak engellerle karşılaştığında kırılma, yansıma, saçılma ve sönümleme gibi etkilerle yön değiştirebilir veya zayıflayabilir. Bu yayılım karakteristikleri, kablosuz haberleşmenin performansını doğrudan etkiler.
- **Kanal Kapasitesi ve Bant Genişliği**: Kablosuz bir kanalın kapasitesi, birim zamanda iletebileceği veri miktarını ifade eder. Kanal kapasitesi, kullanılan frekans bandının genişliği (band genişliği) ve modülasyon tekniğine bağlıdır.
- **Hata Düzeltme ve Güvenlik**: Kablosuz iletişimde, sinyaller gürültü ve parazitlere maruz kalabilir. Hata düzeltme teknikleri, iletim sırasında oluşabilecek hataları tespit etmek ve düzeltmek için kullanılır. Ayrıca, veri güvenliğini sağlamak için şifreleme ve kimlik doğrulama yöntemleri uygulanır.


Bu prensipler, kablosuz haberleşme sistemlerinin tasarımını ve işletimini yönlendiren temel unsurlardır. Bu prensiplerin doğru bir şekilde uygulanması, güvenilir ve verimli kablosuz iletişim sağlamak için gereklidir.



## Wi-Fi
Kablosuz yerel ağ olarak Türkçeye çevirebileceğimiz bu kısaltma, Wireless Fidelity sözcüklerinin ilk iki harflerinden oluşmaktadır. 2.4 GHz ve 5 GHz frekanslarında çalışır. IEEE 802.11 standartlarını kullanan tüm cihazlar WiFi cihaz olarak tanımlanabilir. Internet bağlantısı, ev veya işyeri ağı ve iki cihaz arasında haberleşmede kullanılabilir. 



WiFi cihazların temelde 3 farklı çalışma modu bulunur: Infrastructure (altyapı) ve Ad-Hoc (iki cihaz arası doğrudan haberleşme). Infrastructure modunun ise iki farklı alt modu vardır: istemci (client) ve istasyon (access point). İstemci olarak bilgisayarlarımızı, cep telefonlarımızı ve projelerimizde kullanabileceğimiz WiFi modülleri örnek olarak verebiliriz. İstasyon cihazları ise, modem ve router’lardır. Çoğu cihaz istemci ve istasyon moduları arasında değiştirilerek kullanılabilir. Örneğin akıllı telefonumuzdaki kablosuz erişim noktasını açtığımızda telefonumuzun WiFi modülü istemci modundan çıkarak istasyon moduna girmekte ve mobil interneti kendi WiFi modülünü kullanarak yayına sokmaktadır. Endüstriyel alanda kullanılan **Wireless M-Bus USB adaptörü** veya **Wireless M-Bus Modülü** çeşitli Wi-Fi Modülleri arasında yer almaktadır.

Ad-Hoc bağlantıda ise iki cihaz sadece birbiri ile haberleşebilir. Bu durumda iki cihaz da hem istemci hem de istasyon görevi görür.

### IEEE 802.11 standartlarının günümüzde en çok kullanılanları 802.11b/g/n ve ac standartlarıdır.

- 802.11b ve 802.11g standartları, 2.4 GHz frekansını kullanır. Çıkabilecekleri maksimum iletişim hızları, 802.11b standartı için 11 Mbps, 802.11g standartı için 54 Mbps’dir.
- 802.11n standartı, 2.4 GHz ve 5 GHz frekanslarını kullanır. Bu standartı kullanarak çıkılabilecek maksimum hız ise 150 Mbps’dir.
- 802.11ac standartı 5 GHz frekansını kullanır. Bu standartı kullanarak çıkılabilecek maksimum hız ise 780 Mbps’dir.

- **Teknolojiler:** IEEE 802.11 standartları ailesine dayanır. Wi-Fi 4 (802.11n), Wi-Fi 5 (802.11ac) ve Wi-Fi 6 (802.11ax) en yaygın versiyonlarıdır.
- **Frekans Bantları:** 2.4 GHz ve 5 GHz bantları; Wi-Fi 6E ile 6 GHz bandı da kullanılmaya başlanmıştır.

## Bluetooth

Kısa mesafelerde veri transferi için geliştirilmiş bir teknolojidir. İlk çıktığında RS-232 bağlantıya kablosuz bir alternatif olması için Ericsson tarafından 1994 yılında geliştirilmiştir. 2.4 GHz frekansında çalışır. Dosya transferi, ses aktarımı ve sanal COM portu gibi uygulamalarda kullanılır. İletişim protokolü sürekli gelişmekte ve güncellenmektedir. Güncel cihazlar yeni protokolleri desteklediği gibi, geriye dönük uyum da mevcuttur.

### Bluetooth haberleşmede hızlar şu şekildedir:

- Bluetooth v1.2 : 1 Mbps
- Bluetooth v2.0+EDR : 3 Mbps
- Bluetooth v3.0+HS : 24 Mbps
- Bluetooth v4.0: 24 Mbps




Günümüzde akıllı saatler gibi az güç tüketmesi hedeflenen cihazlar ise Bluetooth Low Energy isimli protokolu kullanmaktadır. Bu protokol, sadece Bluetooth v4.0 ve BLE destekleyen cihazlarla uyumludur, geriye dönük uyumluluğu yoktur.

- **Teknolojiler:** Bluetooth Low Energy (BLE) düşük enerji tüketimi sağlar ve IoT cihazlarında yaygın olarak kullanılır.
- **Frekans Bandı:** 2.4 GHz ISM bandı.


## Hücresel Ağlar

- **Teknolojiler:**
2G: GSM, EDGE; temel ses ve düşük hızda veri hizmetleri.
3G: UMTS, CDMA2000; orta hızda veri hizmetleri.
4G: LTE; yüksek hızlı internet ve geniş bant veri hizmetleri.
5G: Gelişmiş hız, düşük gecikme ve yüksek bağlantı yoğunluğu ile en yeni nesil.
- **Kullanım Alanları:** Mobil telefonlar, tabletler, IoT cihazları ve mobil geniş bant hizmetleri.
- **Frekans Bantları:** 700 MHz – 2.6 GHz (4G) ve 24 GHz – 40 GHz (5G) arası değişen geniş frekans bantları.



## NFC ve RFID

NFC(Near Field Communication), çoğunlukla RFID ile karıştırılmaktadır. RFID, genel anlamıyla nesnelerin radyo dalgaları kullanılarak tanınması için kullanılan teknolojiye verilen addır. Aktif ve pasif tag’leri bulunur. Aktif tag’ler kendi güç kaynağını barındır ve bu sayede daha uzak mesafelerden haberleşme olanağı sunar. Pasif tag’ler okunma sırasında oluşan manyetik alandan beslenerek çalışırlar. Aktif ve pasif tag’lere en güzel örnek olarak, köprü ve otoyol gişelerinde kullanılan OGS ve HGS sistemleri verilebilir. OGS, cihazı içinde pil barındıran büyük bir cihaz iken HGS kart veya etiket şeklindedir. Üç farklı frekans bandında çalışan RFID tag’leri bulunmaktadır:

- Low Frequency (LF) 125 -134 kHz
- High Frequency (HF)13.56 MHz
- Ultra High Frequency (UHF) 856 MHz to 960 MHz
- NFC, 10 cm gibi kısa mesafelerde cihazları birbirine dokundurarak veya yaklaştırarak çalışan bir kablosuz haberleşme teknolojisidir. NFC, RFID teknolojisinin bir uygulamasıdır. HF bandında (13.56 MHz) çalışır.


NFC cihazlar üç farklı modda çalışabilir: NFC kart emülasyon modu, yazıcı/okuyucu modu ve peer-to-peer modu. Kart emülasyon modunda akıllı telefon gibi cihazlar kart gibi davranarak alışverişte ödeme yapma vb. şekillerde kullanılabilir. Yazıcı/okuyucu modunda, NFC cihaz bir NFC kartı yada tag’i okuma ve yazmada kullanılabilir. Peer-to-peer modunda ise iki NFC cihaz arasında dosya aktarımı gibi protokoller, NFC kullanılarak başlatılır.

NFC kartlar küçük miktarda belleğe sahiptir. Bu bellek sadece okunabilir yada tekrar yazılabilir yapıca olabilir. Kısa mesafeli ödeme sistemleri, kimlik doğrulama ve veri transferi (örneğin, temassız kredi kartları, akıllı telefon ödemeleri) alanlarında kullanılır. Frekans Bandı, 13.56 MHz'dir.


## Uydu İletişimi:

- **Kullanım Alanları:** Küresel iletişim, yayıncılık, GPS (küresel konumlama sistemi), uzaktan veri aktarımı.
- **Frekans Bantları:** L-bandı, S-bandı, C-bandı, X-bandı, Ku-bandı ve Ka-bandı gibi çeşitli frekanslar.




## Zigbee Modülleri
Zigbee modülleri sağladığı düşük güç tüketimi ve geniş kapsama alanı gerektiren uygulamalar için tasarlanmış kablosuz haberleşme teknolojisidir. Endüstriyel otomasyon, enerji yönetimi, akıllı ev sistemleri ve sensör ağları gibi IoT tabanlı çözümlerde yaygın olarak kullanılır. Zigbee modülleri, mesh ağ topolojisini destekleyerek cihazlar arasında doğrudan veya dolaylı olarak veri aktarımı sağlar, böylece ağdaki cihaz sayısı arttıkça kapsama alanı genişler ve iletişim güvenliği artar.

- **Kullanım Alanları:** Düşük güç tüketimi gerektiren ve düşük veri hızına ihtiyaç duyan IoT uygulamaları (örneğin, ev otomasyonu, sensör ağları).
- **Frekans Bandı:** 2.4 GHz ISM bandı.


## Z-Wave:

- **Kullanım Alanları:** Ev otomasyonu, güvenlik sistemleri ve enerji yönetimi.
- **Frekans Bandı:** 908.42 MHz (ABD), 868.42 MHz (Avrupa).




### Bunlar dışında diğer kablosuz haberleşme standartları(modülleri): XBee, LoRaWAN, NM-IoT, 


---

## Kablosuz Haberleşme Modülü Seçerken Dikkat Edilmesi Gerekenler
Endüstriyel uygulama alanları, sayaç okuma sistemleri veya akıllı ev çözümlerinizde kablosuz haberleşme modülü seçerken aşağıdaki bazı adımlara dikkat edilmesi gerekebilir;

- Kapsam Alanı ve Mesafe
- Güç tüketimi
- Veri Hızı ve Bant Genişliği
- Güvenlik Özellikleri
- Maliyet ve Ekonomik Değerlendirme



### Kapsam Alanı ve Mesafe
Bir haberleşme modülünün kapsam alanı, cihazlar arasında sağlanan maksimum iletişim mesafesini belirler ve uygulamanın gereksinimlerine göre değişiklik gösterir. Örneğin, akıllı ev sistemlerinde Wi-Fi veya bluetooth gibi modüller yeterli olurken, tarım veya çevresel izleme gibi uzun mesafeli ve geniş kapsamlı uygulamalarda LoRaWAN veya Zigbee gibi uzun menzilli modüller tercih edilebilir. Kapsama alanı ve mesafe, sinyal gücü, ortam koşulları ve engeller gibi faktörlerden de etkilenir; bu nedenle, modül seçiminde bu unsurların da göz önünde bulundurulması gerekir. Uygulamanın ihtiyaç duyulan kapsama alanına uygun şekilde bir modül seçimi yapılması veri güvenliği ve performans açısından fayda sağlar.

### Güç Tüketimi
Haberleşme modülü seçiminde güç tüketimi önemli bir faktördür. Modülün ihtiyaç duyduğu enerji ihtiyacı, cihazın batarya ömrünü doğrudan etkilediği için özellikle pil ile çalışan IoT cihazları, taşınabilir elektronikler ve sensörler gibi uygulamalarda önem taşır. Düşük güç tüketimine sahip modüller cihazların daha uzun süreli ve kesintisiz çalışmasını sağlar, bu sayede bakım ve pil değiştirme maliyetlerini azaltır. Güç tüketimi, modülün aktif, uyku ve bekleme modlarında ki enerji ihtiyacına göre değerlendirilmelidir.

### Veri Hızı ve Bant Genişliği
Veri hızı modüllerin veri iletimi ve nesnelerin haberleşme hususunda önemli bir faktördür. bir modülün belirli bir süre içerisinde ne kadar veri iletebileceğini ifade ederken, bant genişliği ise bu verilerin iletilmesi için kullanılan frekans aralığını belirler. Endüstriyel veya ev tipi uygulamaların gereksinimlerine göre doğru veri hızı ve bant genişliği sistemin performansını doğrudan etkileyen önemli bir faktördür. Örneğin, enerji verimliliğinin daha önemli olduğu ve düşük veri hızı gerektiren IoT uygulamaları için Zigbee veya LoRaWAN gibi modüller tercih edilebilir. Yanlış seçilen bir veri hızı veya bant genişliği, ya gereksiz enerji tüketimine neden olabilir ya da sistemin verimli çalışmasını engelleyebilir. Bu nedenle uygulamalarınızın ihtiyaç duyduğu modülleri seçmek önemlidir.

### Güvenlik Özellikleri
Kablosuz iletişim sırasında, verilerin cihazlar arasında güvenli bir şekilde iletilmesi oldukça önemlidir. Bu hususta seçilecek olan haberleşme modülünün güvenlik standartlarını karşılayıp karşılamadığı kontrol edilmelidir. Güvenlik özellikleri, verilerin izinsiz erişim, dinleme, müdahale ve saldırılara karşı korunmasını sağlar. Güvenlik önlemleri arasında veri şifreleme, kimlik doğrulama protokolleri, güvenli anahtar yönetimi ve güvenli veri iletim mekanizmaları bulunur. Örneğin, Zigbee ve LoRaWAN modülleri güçlü güvenlik standartlarıyla donatılmıştır, Ayrıca Wİ-Fİ modülleri de genellikle WPA3 gibi gelişmiş şifreleme protokolleri sunar. Dolayısıyla uygulamaların güvenlik gereksinimlerine uygun bir modül seçimi, veri bütünlüğünü korur, yetkisiz erişimi engeller ve cihazlar arasındaki iletişime güvenli kılar.

### Maliyet ve Ekonomik Değerlendirme
Haberleşme modülünün maliyeti, başlangıçtaki satın alma fiyatını değil, aynı zamanda uzun vadede işletim ve bakım maliyetlerini de kapsar. Uygulamanın bütçesine uygun modül seçimi ekonomik anlamda avantajlı kılabilir fakat düşük maliyetli modüller daha cazip gelse de uzun vade de sürdürülebilir olmayabilir. Dolayısıyla maliyet-fayda dengesi göz önüne alınarak projeye uygun bir modül seçimi yapılması daha uygundur. HDA Enerji markasının sunmuş olduğu haberleşme modülleri projelerinize uygun, sürdürülebilir ve uzun vadeli çözüm sağlamayı amaçlamıştır.




---


## Iot Uygulamaları İçin Kablosuz Haberleşme Modülleri

Kablosuz haberleşme modülleri, IoT uygulamalarında sıklıkla kullanılan bir teknolojidir. Cihazların birbirleriyle iletişim kurabilmesini sağlayan bu modüller aşağıda bulunan uygulamalarda kullanılabilir:

- Akıllı Ev Sistemleri(Wi-Fi, bluetooth, Zigbee)
- Endüstriyel Otomasyon(LoRaWAN, Zigbee, Wi-Fi, bluetooth)
- Sağlık İzleme Sistemleri(Wi-Fi, Zigbee, bluetooth)
- Akıllı Şehir Çözümleri(LoRaWAN, Wi-Fi, 5G, Zigbee)
- Enerji Yönetimi ve İzleme(LoRaWan, Zigbee, 5G, Wi-Fi) 



# KAYNAKÇA
- https://www.hdaenerji.com.tr/kablosuz-haberlesme-modulleri-ve-iot/
- https://maker.robotistan.com/kablosuz-haberlesme-teknolojileri/
- https://emanetemre.medium.com/kablosuz-haberle%C5%9Fme-teknolojileri-19d08a899d02
- https://www.techtarget.com/searchmobilecomputing/definition/wireless
- https://askweb.com.tr/kablosuz-haberlesme-nedir-kablosuz-haberlesme-teknolojileri/
