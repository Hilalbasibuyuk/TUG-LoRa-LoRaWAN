## TUG-LoRa-LoRaWAN

LoRa, ‘Long Range’ yani ‘Uzun Mesafe’ kelimelerinin ilk hecelerinden ismini almaktadır. Nesnelerin İnterneti (Internet of Things, IoT) uygulamalarının son on yılda tüm dünyada büyük hızla yayılmasıyla birlikte, verilerin uzak mesafeye güvenilir ve düşük güç tüketimiyle aktarılması önemli bir ihtiyaç haline gelmiştir. Son dönemde ise bu ihtiyaca cevap verebilecek haberleşme teknolojilerinde önemli gelişmelere tanık oluyoruz. Bu gelişmelerin başında ise, LoRa, Sigfox, NB-IOT gibi, düşük bit oranlarındaki verinin uzun mesafelere düşük güç tüketimiyle aktarımını sağlayan kablosuz haberleşme teknolojilerinin ortaya çıkışı geliyor.

Bu teknolojiler arasında en fazla yaygınlık kazanan LoRa, WiFi ve kablolu haberleşme gibi rakip teknolojilere göre çok daha uzun mesafede iletişim sağlayan, ve bunu radyo frekanslarını kullanarak gerçekleştiren bir modülasyon tekniğidir. LoRaWAN (Long Range Wide Area Network) ise bölgesel, ulusal veya küresel ölçekte bir ağ üzerinde kablosuz olarak çalışan ürünlere yönelik tasarlanmış, düşük güçlü geniş alan ağı belirtimidir. 




<img width="834" height="706" alt="image" src="https://github.com/user-attachments/assets/60187df3-a788-4a1a-a4e9-6afcd7b2029d" />



Resim kaynakçası -> https://blog.direnc.net/lora-ve-lorawan-nedir/



### LoRa Neden Geliştirildi?
Nesneleri internete bağlamak amacıyla halihazırda kullanılmakta olan hücresel haberleşme (2G, 3G, 4G +) ve WiFi gibi yöntemlerin son zamanlarda uzun mesafede veri iletimi veya bu iletimin sürekliliği gibi ihtiyaçları tam olarak karşılayamaması, ya da bu ihtiyaçları karşılarken yüksek maliyet ortaya çıkarması, bu dezavantajları giderebilecek yeni teknoloji arayışının itici gücü olmuştur. WiFi teknolojisindeki mesafe sınırlaması, hücresel haberleşmenin maliyetleri ve yüksek enerji kullanımı, LoRa teknolojisiyle önüne geçilmesi gereken temel eksiklikler olarak belirlenmiştir. Bölgesel olarak farklılık gösteren radyo frekansı aralıklarını kullanan LoRa, açık alanda 15 km’ye kadar genişleyebilen bir mesafede bağlantı kurabilirken, uç noktada bağlı cihazlar 8 yıldan 15 yıla kadar sorunsuz olarak iletişimi sürdürebilmektedir.


### LoRa ağı temel özellikleri

- **Uzun Menzil:** LoRa, düşük frekansta (genellikle 868 MHz veya 915 MHz) çalışarak uzun menzil sağlar. Bu sayede,sensörler veya cihazlar daha uzak mesafelerde bulunan gateway'lere (ana cihazlar) veri gönderebilirler
- **Düşük Güç Tüketimi:** LoRa teknolojisi, düşük güç tüketimi ile öne çıkar. Bu özellik, sensörlerin veya cihazların pil ömrünü uzatır ve enerji tasarrufu sağlar.
- **Yüksek Kapasite:** LoRa ağları, çok sayıda cihazın aynı anda çalışmasına izin verir. Bu, büyük ölçekte IoT uygulamaları için uygundur.
- **Düşük Maliyet:** LoRa ağları, düşük maliyetli çipler ve ekipmanlar kullanarak ekonomik bir çözüm sunar
- **Açık Standart:** LoRa, açık bir standarttır ve bu nedenle birçok farklı cihaz ve uygulama tarafından desteklenir.

---

LoRa haberleşme teknolojisinin kullanımı için en uygun alanlar, veri büyüklüğünün düşük veya orta seviyede olduğu, aktarımda yaşanabilecek kısa süreli gecikmelerin göz ardı edilebileceği, bir başka deyişle, “mission-critical” olarak da tabir edilen yaşamsal altyapı sistemlerinin dışında kalan uygulama alanlarıdır. Bu alanlara en iyi örnek akıllı tarım uygulamalarıdır. Uzun süre bakıma ihtiyaç duymadan geniş alanlara sinyal aktarımı yapabilen LoRa teknolojisi sayesinde akıllı tarım uygulamaları çok daha kolay takip edilebilir ve geliştirilebilir hale gelmiştir. Toprak kirliliği, nem, sıcaklık ve güneş ışığı gibi etkenleri ölçmek üzere konumlandırılan LoRa destekli sayaçlar ile uzak bir konumdan tarım alanının uygun şartlarda olup olmadığı kontrol edilebilir hale gelecektir. Akıllı tarımın yanı sıra küçük veri paketlerinin söz konusu olduğu su ve gaz sayacı uygulamaları, fabrika otomasyonu veya akıllı bina uygulamaları da LoRa’nın rahatlıkla kullanılabileceği alanlardır. ​

### LoRa ağı genellikle şu uygulamalarda kullanılır:

- Akıllı şehir uygulamaları (park sensörleri, çöp kutuları, aydınlatma kontrolü)
- Endüstriyel IoT (fabrika otomasyonu, tarım sensörleri)
- Uzaktan sensör izleme ve kontrol
- Akıllı tarım projeleri (yukarıda bahsettik)
- Ev otomasyonu ve akıllı bina sistemleri


LoRa, geniş alanlarda dağılmış sensör ağları kurmak isteyen uygulamalar için etkili bir çözümdür



### LoRa Haberleşme Yapısı, Avantaj ve Dezavantajları


LoRa,  temelde dört kısımdan oluşan bir haberleşme teknolojisidir. Birinci kısım **LoRa Node (düğüm noktası)** olarak adlandırılan uç noktalardır. Bu noktalarda LoRa modülü içeren veya modül uyumluluğu sayesinde daha sonra bünyesine LoRa modülü takılabilen sensörler, sayaçlar, kontrol cihazları gibi uç nokta cihazları kullanılır. 


<img width="800" height="800" alt="P1010618_800X800" src="https://github.com/user-attachments/assets/0740f1fb-29b4-4172-a4f8-9d3c70a57573" />



İkinci kısımda **LoRa Gateway** olarak adlandırılan ağ geçidi özelliğindeki cihazlar bulunur. Bu cihazlar, LoRa düğüm noktalarından gelen verileri herhangi bir protokol dönüşümü yapmaksızın Ethernet, WiFi veya hücresel haberleşme gibi haberleşme teknolojilerini kullanarak LoRaWAN sunucusuna aktarır. Robustel tarafından geliştirilen R3000 LG serisi de, bu tür uygulamalarda LoRa Gateway olarak kullanılabilecek cihazlardan biridir. R3000 LG, marka bağımsız olarak uç noktadaki LoRa Node cihazları ile LoRaWAN sunucusu arasındaki bağlantıyı sağlar. 


<img width="785" height="750" alt="LoRa-Gateway-F-LG-2XXXDCX" src="https://github.com/user-attachments/assets/b5b8174b-1e6e-4098-b8d2-be354da24ebe" />



LoRa topolojisinin üçüncü kısımda ise **LoRaWAN sunucusu** yer alır. LoRaWAN sunucusu, ağ geçidinden gelen verileri çözümleyerek uygulama sunucusunda kullanılacak protokole çevirir ve kullanıma hazır hale getirir. 

Son olarak dördüncü aşamada yer alan **Uygulama Sunucuları**, düğüm noktasından gelen verilerin kontrol ve takibini yapar.


<img width="584" height="411" alt="image" src="https://github.com/user-attachments/assets/0ee93087-ca16-4c96-a708-4a594055539a" />


Resim kaynakçası -> https://kalitenetwork.com/blog/lora-ve-lorawan-nedir





Star Topology gereği sensörler direkt olarak birbirleri ile haberleşemezler, gateway üzerinden veri alışverişi yaparlar. Sensörler arası direkt veri aktarımının yapılabilmesi için sensörlerin bir parçası olan gömülü mikroişlemcilerde, RadioHead radyo paketi kütüphanesinin kullanılması gerekir. Bu, verilerin direkt aktarımı için nesne yönelimli bir kütüphanedir.

Gatewayler, ağ sunucusuna standart IP bağlantısı ile yani TCP/IP protokolünü kullanarak bağlanır. IP paketi ile RF paketleri arasında dönüşüm yaparak uç cihazlar ve sensörler arasında bir tercüman, bir köprü rolü oynar. Şöyle ki sensörlerden gatewaye gelen veri RF paketi şeklindedir ancak ağ sunucusuna gönderilen verinin IP paketi şeklinde gönderilmesi gerekir. Bu iki paket tipi arasındaki dönüşümden gateway sorumludur. Aşağıdaki yapıyı incelerseniz her şey daha da netlik kazanacaktır.







<img width="885" height="484" alt="image" src="https://github.com/user-attachments/assets/b182fb83-cb40-4187-bd13-95b960874b09" />
Resim kaynakçası -> https://kalitenetwork.com/blog/lora-ve-lorawan-nedir





### LoRa tabanlı end cihazları

<img width="978" height="425" alt="image" src="https://github.com/user-attachments/assets/86885f41-68cc-41d8-ab9a-cc4ee984efc8" />
Resim kaynakçası -> https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/








<img width="1065" height="714" alt="image" src="https://github.com/user-attachments/assets/7e47f46e-f0cc-4d95-a70e-6950a539311e" />




Resim kaynakçası -> https://gsl.com.tr/lora-kablosuz-haberlesmenin-yukselen-yildizi.html





LoRa haberleşme teknolojisinin diğer kablosuz haberleşme teknolojilerine kıyasla en büyük avantajı, geniş mesafeye düşük maliyetle erişim imkanı sağlamasıdır. Önceden belirtildiği üzere WiFi ile erişim kurabileceğimiz alan çok kısıtlıdır ve bununla birlikte güç tüketimi de yüksek seviyededir. Hücresel haberleşme ise mesafe kısıtlamasına tabi olmamasına rağmen yüksek güç tüketimi, operatör firmaların erişim altyapılarının durumuna bağımlılık ve hizmet bedelleri ortaya çıkarmaktadır. Buna karşın LoRa haberleşme teknolojisinin sunduğu, kapalı alanda 2-3 kilometreye, açık alanda 15 kilometreye kadar varan erişim imkanı, uç noktada bağlı olacak cihaza göre bir veya iki adet kalem pil ile 10 yıla kadar sorunsuz bir şekilde çalışabilmektedir.

Son dönemde bir Gateway cihazına bağlanmış olan binlerce LoRa Node cihazlarının kesintisiz veri aktarımı yapabileceği şeklinde yayılan bilgiler, doğruluk payı oldukça sınırlı bilgilerdir. Binler mertebesinde adetlerde cihazın aynı anda LoRa ağı üzerinden veri aktarımında sıkıntıya neden olabilecek faktörlerin başında Duty-Cycle (görev döngüsü) gelir. Her bir LoRa Node cihazı için veri aktarımı sırasında kanalı meşgul etmesi sebebiyle tanımlanan bir maksimum Duty-Cycle değeri mevcuttur.

Duty-Cycle değeri, haberleşmenin kesintisiz olarak sağlanabilmesi için dikkat edilmesi gereken en önemli faktörlerden birisidir. 868 MHz frekans bandını kullanan Avrupa bölgesinde her bir LoRa Node için Duty-Cycle %1, yani saat başına 36 saniyedir. Bu 36 saniye her bir LoRa Node cihazının bir frekans kanalını bir saat içerisinde meşgul edebileceği en yüksek süredir. Gateway’e bağlanan LoRa Node sayısı arttıkça, iletimi sağlanan paket miktarı, çakışmalardan dolayı azalmaktadır.


<img width="1669" height="503" alt="image" src="https://github.com/user-attachments/assets/c06bad45-ee57-490b-85e4-d138e5b377d5" />



Resim kaynakçası -> https://gsl.com.tr/lora-kablosuz-haberlesmenin-yukselen-yildizi.html




LoRa’nın, LoRa uç cihazları ve LoRaWAN’dan oluştuğundan bahsetmiştik. Aşağıdaki görsele baktığımızda da bunun bir özetini görüyoruz. RF layer, kullanılacak radyo frekansı aralığının tanımlandığı katmandır. Physical Layer yani fiziksel katmanda ise LoRa uç cihazları bulunmaktadır. LoRa protokolünde fiziksel katmanda, LoRa uç cihazları ve Gateway arasında sadece tek bir “hop” bağlantısınayani atlama adımına izin verilir. LoRaWAN kısmına ise ağda bulunan cihazların sınıf bilgisi ve uygulama katmanı dahildir.



<img width="599" height="334" alt="image" src="https://github.com/user-attachments/assets/409ab325-4954-4d86-b7da-658812d4fa1a" />



Resim kaynakçası -> https://kalitenetwork.com/blog/lora-ve-lorawan-nedir

---

## LoRa Katılım Prosedürü
LoRa iletişim ağına katılan yeni bir cihazın aktivasyonu, aşağıda listelenen iki işlemden herhangi biri ile tamamlanabilir.:

- Kişiselleştirme ile Aktivasyon (ABP)
- Havadan Aktivasyon (OTAA)
Aktivasyon işleminin sonunda, hem Ağ oturum anahtarı hem de Uygulama oturum anahtarı yeni cihazla paylaşılırdı, şimdi Son düğüm cihazı olarak anılacak olan.

### Kişiselleştirme ile etkinleştirme (ABP)
LoRa ağına katılmanın ABP yöntemi, AppEUI gibi bazı belirli oturum anahtarlarına sahip olmadan yeni bir cihazın eklenmesini içerir., DevEUI, vb. onunla paylaştı. Bunun yerine, dahil olmak üzere oturum anahtarları, FNwk_SIntKey ve yaklaşık üç kişi daha, doğrudan Son cihazda depolanır. Bir cihaz, yalnızca LoRa ağ katılımı gerekli bilgilerine sahipse ABP işlemi aracılığıyla etkinleştirilebilir., başlangıçta.

### Havadan Aktivasyon (OTAA)
Kablosuz etkinleştirme prosedürü, bir Uç Cihaz ile Ağ sunucusu arasındaki doğrudan iletişimi içerir.. Bu etkinleştirme işlemi yalnızca Sonlandırma cihazı sıfırlandığında tercih edilir.

OTAA süreci şunları içerir::

Yeni cihaz, LoRaWAN ağına istekte bulunan belirli bir mesajı LoRa ağ sunucusuna gönderir..
Ağ sunucusu mesajı alır ve geçersiz veya geçerli olarak yorumlar.. geçerliyse, bir kimlik doğrulama veya oturum anahtarı oluşturulur



---


### LORAWAN Haberleşme Sistemi

LoRaWAN yani Long Range teknolojisi ile haberleşme yapan LoRa sensörleri ve lora kontrolörleri LoRa gateway cihazı ile kablosuz irtibatlamak suretiyle sahadan veri toplamak ve sahaya komut vermek için kullanılan sistemerdir.
Sahadan gelen tüm veriler LoRa gateway üzerinden bir LoRa IoT bulut platformuna gönderilir. Bu cloud platformu istenen analizleri yapar ve gerekirse sahaya otomtik olarak belli koşullara bağlı komutlar gönderebilir.
Örneğin seraların yer aldığı bir sahada, sera içindeki nem oranı düştüğünde, lora nem sensörü bu değeri LoRa geçit cihazı vasıtasıyla iot bulut platformuna iletir. Bu durum bulut platformunun sahadaki lora controller cihazını tetiklemesine yol açar ve kontroller su vanasını çalıştırır.
Ayrıca sahadaki modbus sistemler de LoRa kablosuz ağı üzerinden SCADA sistemine entegre edilebilir.



## LoRaWAN Sınıfları


<img width="744" height="717" alt="image" src="https://github.com/user-attachments/assets/64a5db7c-e89b-412a-a112-501a06f5aa51" />


Resim kaynakçası -> https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/#elementor-toc__heading-anchor-50



### A Sınıfı (Tetikleme ile dinleme, Düşük Pil Tüketimi)
Tüm LoRa cihazlar A sınıfı ile uyumludur. A sınıfı cihazlarda pil tüketimi en az seviyede tutularak güç konusunda büyük oranda tasarruf sağlamak esastır. Uç cihazlar (sensörler) sürekli olarak gateway’e (ağ geçidi) mesaj gönderebilirler. Yani uplink (uç cihaz -> gateway) sürekli olarak yapılabilir ancak cihazlar ağı dinleme anlamında sürekli uyku modundadır. Güç konusundaki büyük avantaj bu durumdan kaynaklanır. Çünkü uç cihazlar ağı dinlemek için bir pil tüketimi gerçekleştirmez. Bu sebeple gatewayden uç cihaza mesaj iletimi her zaman olamaz. Bir downlink (gateway -> uç cihaz) sadece bir uplink sonrasında gerçekleştirilebilir. Gateway uç cihazdan gelen veriyi servera (sunucu) yönlendirir. Sunucudan ise verinin alındığına dair bir ACK mesajı + gerekli yanıt döner, gateway bunu uç cihaza LoRa paketi halinde sunar. Böylece bir uplink işleminin hemen ardından bir downlink gerçekleştirilmiş olur.

LoRa haberleşme teknolojisinin diğer kablosuz haberleşme teknolojilerine kıyasla en büyük avantajı, geniş mesafeye düşük maliyetle erişim imkanı sağlamasıdır. Önceden belirtildiği üzere WiFi ile erişim kurabileceğimiz alan çok kısıtlıdır ve bununla birlikte güç tüketimi de yüksek seviyededir. Hücresel haberleşme ise mesafe kısıtlamasına tabi olmamasına rağmen yüksek güç tüketimi, operatör firmaların erişim altyapılarının durumuna bağımlılık ve hizmet bedelleri ortaya çıkarmaktadır. Buna karşın LoRa haberleşme teknolojisinin sunduğu, kapalı alanda 2-3 kilometreye, açık alanda 15 kilometreye kadar varan erişim imkanı, uç noktada bağlı olacak cihaza göre bir veya iki adet kalem pil ile 10 yıla kadar sorunsuz bir şekilde çalışabilmektedir.

<img width="787" height="431" alt="image" src="https://github.com/user-attachments/assets/6a120dcb-5667-4e01-a53c-a27422f9eff3" />
Resim kaynakçası -> https://kalitenetwork.com/blog/lora-ve-lorawan-nedir


A Sınıfı cihazlar özellikle sürekli veri aktarımının olmadığı, tetikleyici bir işlem sonrasında hemen yanıt alınması istenen uygulamalarda kullanılır.

Özetle A sınıfı cihazlar sürekli mesaj, veri gönderebilirler(uplink) ancak mesaj, veri alımını (downlink) sadece bir uplink gerçekleştirdikten sonra yapabilirler.

### B Sınıfı (Periyodik Dinleme, Dengeli Pil Tüketimi)
B Sınıfı cihazlarda zamanlanmış veri iletişimi gerçekleşir. B Sınıfı bir cihazın bir veri alabilmesi için gateway’den periyodik olarak yani belirli zaman dilimlerinde senkronize olduklarına ilişkin bir işaret sinyali (beacon) alması gerekir. Uç cihaz ve gateway’in senkronize olmadığı anlarda bir uç cihaza veri iletimi yani downlink gerçekleştirilemez. Yine aynı şekilde uplink de sadece bu belirli zaman aralıklarında gerçekleştirilebilir.

Özetle B sınıfı cihazlar, mesaj gönderme ve alma işlemlerini sadece ayarlanmış zaman dilimlerinde gerçekleştirebilirler.



### C Sınıfı (Sürekli Zamanlı Dinleme, Yüksek Pil Tüketimi)
Bu sınıfa dahil olan cihazlarda sürekli olarak dinleme gerçekleştirilir böylece herhangi bir zaman diliminde downlink gerçekleştirilebilir. Yani mesaj alımları periyodik değil sürekli olarak gerçekleşir. Böylece gecikmesiz, gerçek zamanlı şekilde veri aktarımı gerçekleştirilebilir. Bu olması istenen durumdur ancak sürekli dinleme sebebiyle yüksek pil tüketimi olduğundan sadece gerçek zamanlı veri aktarımının kritik olduğu uygulamalarda kullanılır.

Özetle C Sınıfı cihazlar, sürekli olarak mesaj alıp gönderebilirler.

### Kimlik Sunucusu
Kimlik sunucusu, LoRa ağına katılan kullanıcıların kimliğini tespit eder. Bir LoRaWAN ağında, Kimlik sunucusu cihazları kaydeder, ağ geçitleri, kullanıcılar ve uygulamalar. Bir bakıma, Identity, LoRaWAN ağının belkemiğidir, çünkü birden fazla cihazda ve dünyanın farklı yerlerinde çalışabilmesini sağlar..


### Ağ Bileşenleri ve İşleyiş

- **Uç cihazlar (end nodes)**: Sensör gibi aygıtlardır, genellikle pil ile çalışır ve düşük enerjiyle veri gönderir. 

- **Ağ geçitleri (gateways)**: Uç cihazlardan gelen sinyalleri alır, internet backbone’una iletir. 

- **Ağ sunucusu**: Verilerin yönlendirilmesini, kimlik doğrulamasını ve güvenliği sağlar. 

- **Uygulama sunucusu**: Nihai verilerin çözümlenip kullanıma sunulduğu katmandır.



### Modülasyon
LoRa, Chirp Spread Spectrum'dan türetilen yayılı spektrumun patent modülasyon projesidir.. Chirp yayılma spektrumu, hassasiyet için belirli bir bant genişliği içinde iletimin veri hızını değiştirerek LoRaWAN iletişim ağının frekansını modüle eder.. Bu, ağın verimliliğini optimize eder ve aynı zamanda belirli bir bant genişliğini korurken aynı zamanda LoRa ağının iletişim aralığını genişletir..



### Tablo

<img width="741" height="459" alt="image" src="https://github.com/user-attachments/assets/92223eef-55af-4bc2-9bf3-292a33c62295" />
Resim kaynakçası -> https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/#elementor-toc__heading-anchor-50


LoRaWAN Ağı, lisanslı veya lisanssız olabilen Radyo kablosuz frekans bantları üzerinden iletişim iletir.. Lisanssız Radyo frekansları ücretsizdir ancak, lisanslı frekanslara kıyasla parazite karşı daha hassastır.

LoRa ve LoRaWAN iletişiminin etkinliğinin sırrı, veriler belirli bir frekans üzerinden iletilirken Frekansları modüle etmek için Chip Spread spektrumunu kullanan LoRaWAN iletişim ağının dahice tasarımıdır.. Öyle bir şekilde ki, LoRa iletişimleri bile lisanssız Radyo Frekansı üzerinden çok az veya hiç girişim şansı yok. Eşzamanlı olarak bağlantıyı daha ucuz ama daha verimli hale getirir ve verilerin uzun mesafelerde iletilmesine olanak tanır.

LoRa ve LoRaWAN iletişim ağlarında, belirli frekanslar, birçok farklı LoRa uygulamasına özgü LoRa radyoları ve LoRa saatleri aracılığıyla yapılandırılabilir.

**Lisanssız MHz Radyo Frekanslarına Bazı Örnekler:**

- Asya: 169MHz, 433MHz

- Kuzey Amerika: 915 MHz


### Lisanssız Frekans kullanan LoRa için düzenleyici hususlar
LoRa ve LoRaWAN, radyo frekans bantları üzerinden veri iletişimi iletirken. LoRa Ağı öncelikle lisanssız frekansları kullanır, yani, aracılığıyla sinyal yayınlamak için bir devlet lisansı almanız gerekmeyen bu frekanslar. Lisanssız frekanslar, her coğrafi bölgeye ve konuma özeldir.. Güvenlik ve verimlilik amaçları için. Her bölgenin hükümeti, bulunduğunuz yerde belirtilmeyen frekans bandı üzerinden yayın yapmaktan büyük ölçüde hoşnut değildir.. Öyleyse, LoRa ağını kullanırken, LoRa telsizleriniz ve saatleriniz, bulunduğunuz yere özel frekans bantlarına göre yapılandırılmalıdır.


### LoRaWAN bant genişliği değerlendirmesi

<img width="841" height="425" alt="image" src="https://github.com/user-attachments/assets/21c699e1-4aee-4e11-b4ce-af968ed23ab2" />
Resim kaynakçası -> https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/#elementor-toc__heading-anchor-50


LoRaWAN ağı Veri aktarım hızının sınırı yaklaşık 100 bayt, Tek bir Uç düğüm cihazı ve ağ geçidi arasında bir seferde yalnızca bu kadar veri yükü etkin bir şekilde iletilebilir. LoRaWAN ağı genellikle uç çoklu uç düğüm cihazları ve tek bir ağ geçidi arasında eşzamanlı iletişimi içerir..



### Uyarlanabilir veri hızı

<img width="429" height="147" alt="image" src="https://github.com/user-attachments/assets/b4e01e07-20b5-435f-8bf2-5b725476a582" />
Resim kaynakçası -> https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/#elementor-toc__heading-anchor-50



LoRaWAN iletişim ağının veri hızı, daha fazla hassasiyet için veri hızı alışverişinde dinamizmi ve ayrıca yalnızca belirli verilerin Ağ seçimi anlamında uyarlanabilir., LoRaWAN iletişiminde azaltılmış veri hızına yol açar. Yayılı spektrum modülasyonlu LoRaWAN frekansı, farklı veri hızlarının birbiriyle karışmasını önler. Böylece, ağ geçitlerinin ve genel ağın verimliliğini optimize etmek.



### LoRa aralığı

<img width="588" height="290" alt="image" src="https://github.com/user-attachments/assets/612e131c-9e53-4306-952f-e3f08876dcf7" />
Resim kaynakçası -> https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/#elementor-toc__heading-anchor-50


LoRa teknolojisi, küçük boyutlu verilerin uzun mesafelerde iletimi için menzili artırmak ve güç tüketimini azaltmak için Bant Genişliği konsantrasyonunu azaltmaya dayanmaktadır..

LoRa-Range, fiziksel konumdan da etkilenebilir. Belirli bir LoRaWAN sürümünün menzili, bina kümeleriyle dolu kentleşmiş bir toplulukta daha kısa olacaktır., daha az ve daha fazla aralıklı ek binaya sahip olan ve dolayısıyla, iletim frekansı tıkanıklığında daha az şans.




### LoRaWAN rakiplerinden daha mı iyi?

LoRa ve LoRaWAN iletişim ağları diğerlerinden daha iyi.

LoRaWAN, en yaygın kullanılan Düşük güçlü kablosuz geniş alan ağı olmasının yanı sıra, NB-IoT gibi diğer LPWAN bağlantı seçenekleri LoRaWAN kadar uygun maliyetli değildir. LoRaWAN iletişim ağının bant genişliği, diğer LPWAN'lardan nispeten daha düşüktür ve bu, rakiplerine kıyasla daha fazla kapsama alanı ve daha uzun menzil sağlar.. Ayrıca, LoRaWAN, Farming'deki rakiplerine kıyasla daha geniş bir alanda uygulanabilir., LoRaWAN'ın endüstrilere ve normal ev hizmetlerine sulama için akıllı su sayacında uygulanmasında. LoRaWAN sensörleri ve teknolojisi, LoRa teknolojisinin aşağıdakiler gibi belirli atmosferik koşulları izlemek için kullanılabileceği akıllı bina uygulamasına da genişliyor.; sıcaklık, nem. LoRa teknolojisinin binaların güvenliği ve genel bakımındaki uygulaması da hızla benimseniyor. Buna karşılık, Karşılaştırmada diğer LPWAN'ların uygulanması çok sınırlıdır.



### LoRa ve LoRaWAN'ın Özellikleri
- LoRaWAN ağının bant genişliği 125 kHz
- LoRa tabanlı uç cihazların minimum ortalama pil ömrü, 7 yıllar.
- Ağ geçitlerinin tepe ve uyku akımı yaklaşık 32 sırasıyla mili amper ve 1 mikro amper.
- LoRaWAN ağında iletilen tüm veriler iki kez şifrelenir
- Cihazlar, LoRaWAN ağında yaklaşık 10Km'lik çok uzun bir aralıkta düşük güç tüketimi ile iletişim kurabilir ve veri iletebilir..
- LoRaWAN ağında, veriler radyo frekansı üzerinden aktarılır (Lisanssız frekans bantları daha yaygın olarak kullanılır)
- LoRa ağı, Bitiş düğümleri gibi bileşenlerden oluşur., ağ geçitleri, Ağ sunucuları, Kimlik sunucuları, LoRa uygulamaları ve yazılımı.
- LoRaWAN iletişim ağı çok uygun maliyetlidir.


### Avantajları
- Uzun menzilli iletişim (şehir dışı alanlarda kilometrelerce)
- Düşük enerji tüketimi → uzun pil ömrü
- Girişime karşı dirençli modülasyon yöntemleri sayesinde kararlılık
- Maliyet açısından cazip (lisanssız frekans kullanımı, altyapı maliyeti düşük)


### Dezavantajları
- LoRaWAN iletişim ağının veri hızı düşük → büyük veri aktarımı için uygun değil 
- Veri iletiminin Lisanssız frekans bantları kanalları parazitlere karşı hassas olabilir.
- LoRaWAN ağının tasarımı, büyük veri yükünün iletimini desteklemiyor.
- Uçtan uca paket çözümü sağlayan hazır ürün seçeneklerinin sınırlılığı




### LoRa ve MQTT
MQTT, ağ sunucuları ve ağ geçidi arasındaki iletişimi sağlamak için kullanılır. Veriler, MQTT protokolü ile birden fazla cihaz arasında iletilir. MQTT protokolü genellikle güvenilir olmayan ağlardaki parazitleri azaltmak için kullanılır., kesintilere duyarlı. Sunucu, MQTT aracısına okuma ve yazma yeteneğine sahip bu mesajları ve istemcileri toplar.. Müşterinin yazmak veya abone olmak istediği konuları belirlemesi gerekir.. Tüm konular seçilebilir. Çoğu zaman, MQTT aracısı, sunucunun makinesinde çalışır. Ağ geçidi, cihazdan alınan görünür yükü, bir yukarı bağlantının iletildiği frekans ve zaman gibi ek bilgilerle birlikte yazacaktır.. MQTT, cihazların, bir müşterinin anlayabileceği şekilde basit yollarla konulmuş veri özel LoRaWAN işlemleri için girişimci veri entegrasyonuna yardımcı olur.. MQTT aracısı, iyi yapılandırıldığında tehlikeli ağ geçitlerinin diğer ağ geçitlerinden gelen yukarı bağlantılara erişmesini de engeller.





### LoRa ve LoRaWAN Güvenlik
IoT’de en önemli konulardan biri de kuşkusuz “güvenlik” kavramıdır. Güvenliksiz bir ağa dahil nesneleri evimizde bulundurmak, kapısı olmayan bir evde yaşamaktan çok da farklı değildir. Zira her iki durumda da tüm yabancılara ve kötü olaylara davetiye çıkaran üst düzey zafiyetler mevcuttur. Bu sebeple “Nesnelerin İnternet”i yapısında güvenlik için de önemli çalışmalara yer verilir.

LoRa’da da verilerin güvenliği için 2 ayrı şifreleme kullanılır.

Bunlardan ilki ağ güvenliği için diğeri uygulama katmanının güvenliği içindir. Uç cihaz ile ağ sunucusu arasındaki verilerin güvenli iletişimi için 128 bitlik benzersiz bir ağ oturum anahtarı kullanılır. Uygulama katmanında ise uçtan uça iletişimde 128 bitlik benzersiz bir uygulama oturum anahtarı kullanılır. Bu 128 bitlik anahtarlar AES algoritmaları kullanılarak üretilir.

LoRa haberleşme teknolojisinin veri aktarım oranının düşük olduğunu da herhangi bir uygulamada kullanmadan önce mutlaka göz önünde bulundurmak gerekir. Küresel çapta farklı frekans bantlarını kullanmakta olan LoRaWAN, Avrupa için on adet frekans kanalı tanımlamıştır. Bu on adet frekans kanalından sekizi 250 bps ile 5,5 kbps arasında aktarım sağlayabilen çoklu veri aktarım hızına sahip kanallardır. Bu sekiz kanal dışında 11 kbps veri aktarım hızına ve 50 kbps aktarım hızına sahip FSK kanalı olarak adlandırılan birer kanal daha mevcuttur.

Son dönemde bir LoRa Gateway cihazına bağlanmış olan binlerce LoRa Node cihazlarının kesintisiz veri aktarımı yapabileceği şeklinde yayılan bilgiler, doğruluk payı oldukça sınırlı bilgilerdir. Binler mertebesinde adetlerde cihazın aynı anda LoRa ağı üzerinden veri aktarımında sıkıntıya neden olabilecek faktörlerin başında Duty-Cycle (görev döngüsü) gelir. Her bir LoRa Node cihazı için veri aktarımı sırasında kanalı meşgul etmesi sebebiyle tanımlanan bir maksimum Duty-Cycle değeri mevcuttur.

Duty-Cycle değeri, haberleşmenin kesintisiz olarak sağlanabilmesi için dikkat edilmesi gereken en önemli faktörlerden birisidir. 868 MHz frekans bandını kullanan Avrupa bölgesinde her bir LoRa Node için Duty-Cycle %1, yani saat başına 36 saniyedir. Bu 36 saniye her bir LoRa Node cihazının bir frekans kanalını bir saat içerisinde meşgul edebileceği en yüksek süredir. LoRa Gateway’e bağlanan LoRa Node sayısı arttıkça, iletimi sağlanan paket miktarı, çakışmalardan dolayı azalmaktadır. 


### LoRa Araç Kiti Talimatları
- Arduino IDE'yi kurun ve 340 sürmek
- Kurulu Arduino için bir LoRa kitaplığı yükleyin.
- LG01-N ağ geçidini kurmak için ağ ortamını optimize edin.
- Bileşenleri düzenleyin ve LG01-N ağ geçidini internete en uygun şekilde bağlayın.
- SSH kullanarak LG01-N'ye erişebilmek için bir macun aracı indirin
- LoRaWAN ağını test edin
- TTN sunucusunda bir ağ geçidi kurun
- LG01-N ağ geçidini kurun
- LoRaWAN ağ sunucusuna ağ geçidi bağlantısını kurun.
- Ağ geçidinin LoRa iletişim frekansını kendi konumunuza göre yapılandırın..
- Cayenne uygulama sunucusuyla bağlantı kurun
- LoRa uygulamasından uç cihazlara veri iletişimi ile tekrarı kontrol edin
- Ağ sisteminde sorun giderme.
- LoRa Tabanlı uç cihaz şifrelemesi ve GPS kalkanları kurulumu.
- ABP cihazını TTN'de kurun ve UNO'ya yükleyin




### LPWAN nedir

LPWAN (Low Power Wide Area Network), düşük güç tüketimi ile geniş alan kapsaması sağlayan bir kablosuz haberleşme teknolojisidir. LPWAN teknolojisi, genellikle nesnelerin interneti (IoT) uygulamaları için kullanılır ve düşük bant genişliğine sahip cihazların uzun mesafeler boyunca veri iletmesini sağlar

**LPWAN teknolojisinin popüler örnekleri şunlardır:**

- LoRaWAN: Uzun mesafelerde veri iletimi için kullanılan bir protokol olup, özellikle düşük güç tüketimi ve geniş kapsama alanı sunar

- NB-IoT (Narrowband IoT): Hücresel ağlarla entegre çalışan bir LPWAN teknolojisi olup, düşük veri hızları ve geniş kapsama alanı sunar.



# KAYNAKÇA
- https://gsl.com.tr/lora-kablosuz-haberlesmenin-yukselen-yildizi.html
- https://kalitenetwork.com/blog/lora-ve-lorawan-nedir
- https://gelecekbt.com/lora
- https://blog.direnc.net/lora-ve-lorawan-nedir/
- https://www.mokolora.com/tr/full-understanding-of-lora-and-lorawan/
