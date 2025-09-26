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



### LoRa ağı genellikle şu uygulamalarda kullanılır:

- Akıllı şehir uygulamaları (park sensörleri, çöp kutuları, aydınlatma kontrolü)
- Endüstriyel IoT (fabrika otomasyonu, tarım sensörleri)
- Uzaktan sensör izleme ve kontrol
- Akıllı tarım projeleri
- Ev otomasyonu ve akıllı bina sistemleri


LoRa, geniş alanlarda dağılmış sensör ağları kurmak isteyen uygulamalar için etkili bir çözümdür



### LoRa Haberleşme Yapısı, Avantaj ve Dezavantajları
LoRa,  temelde dört kısımdan oluşan bir haberleşme teknolojisidir. Birinci kısım **LoRa Node (düğüm noktası)** olarak adlandırılan uç noktalardır. Bu noktalarda LoRa modülü içeren veya modül uyumluluğu sayesinde daha sonra bünyesine LoRa modülü takılabilen sensörler, sayaçlar, kontrol cihazları gibi uç nokta cihazları kullanılır. 

İkinci kısımda **LoRa Gateway** olarak adlandırılan ağ geçidi özelliğindeki cihazlar bulunur. Bu cihazlar, LoRa düğüm noktalarından gelen verileri herhangi bir protokol dönüşümü yapmaksızın Ethernet, WiFi veya hücresel haberleşme gibi haberleşme teknolojilerini kullanarak LoRaWAN sunucusuna aktarır. Robustel tarafından geliştirilen R3000 LG serisi de, bu tür uygulamalarda LoRa Gateway olarak kullanılabilecek cihazlardan biridir. R3000 LG, marka bağımsız olarak uç noktadaki LoRa Node cihazları ile LoRaWAN sunucusu arasındaki bağlantıyı sağlar. 

LoRa topolojisinin üçüncü kısımda ise **LoRaWAN sunucusu** yer alır. LoRaWAN sunucusu, ağ geçidinden gelen verileri çözümleyerek uygulama sunucusunda kullanılacak protokole çevirir ve kullanıma hazır hale getirir. 

Son olarak dördüncü aşamada yer alan **Uygulama Sunucuları**, düğüm noktasından gelen verilerin kontrol ve takibini yapar.



<img width="1065" height="714" alt="image" src="https://github.com/user-attachments/assets/7e47f46e-f0cc-4d95-a70e-6950a539311e" />



Resim kaynakçası -> https://gsl.com.tr/lora-kablosuz-haberlesmenin-yukselen-yildizi.html





LoRa haberleşme teknolojisinin diğer kablosuz haberleşme teknolojilerine kıyasla en büyük avantajı, geniş mesafeye düşük maliyetle erişim imkanı sağlamasıdır. Önceden belirtildiği üzere WiFi ile erişim kurabileceğimiz alan çok kısıtlıdır ve bununla birlikte güç tüketimi de yüksek seviyededir. Hücresel haberleşme ise mesafe kısıtlamasına tabi olmamasına rağmen yüksek güç tüketimi, operatör firmaların erişim altyapılarının durumuna bağımlılık ve hizmet bedelleri ortaya çıkarmaktadır. Buna karşın LoRa haberleşme teknolojisinin sunduğu, kapalı alanda 2-3 kilometreye, açık alanda 15 kilometreye kadar varan erişim imkanı, uç noktada bağlı olacak cihaza göre bir veya iki adet kalem pil ile 10 yıla kadar sorunsuz bir şekilde çalışabilmektedir.

Son dönemde bir Gateway cihazına bağlanmış olan binlerce LoRa Node cihazlarının kesintisiz veri aktarımı yapabileceği şeklinde yayılan bilgiler, doğruluk payı oldukça sınırlı bilgilerdir. Binler mertebesinde adetlerde cihazın aynı anda LoRa ağı üzerinden veri aktarımında sıkıntıya neden olabilecek faktörlerin başında Duty-Cycle (görev döngüsü) gelir. Her bir LoRa Node cihazı için veri aktarımı sırasında kanalı meşgul etmesi sebebiyle tanımlanan bir maksimum Duty-Cycle değeri mevcuttur.

Duty-Cycle değeri, haberleşmenin kesintisiz olarak sağlanabilmesi için dikkat edilmesi gereken en önemli faktörlerden birisidir. 868 MHz frekans bandını kullanan Avrupa bölgesinde her bir LoRa Node için Duty-Cycle %1, yani saat başına 36 saniyedir. Bu 36 saniye her bir LoRa Node cihazının bir frekans kanalını bir saat içerisinde meşgul edebileceği en yüksek süredir. Gateway’e bağlanan LoRa Node sayısı arttıkça, iletimi sağlanan paket miktarı, çakışmalardan dolayı azalmaktadır.


<img width="1669" height="503" alt="image" src="https://github.com/user-attachments/assets/c06bad45-ee57-490b-85e4-d138e5b377d5" />



Resim kaynakçası -> https://gsl.com.tr/lora-kablosuz-haberlesmenin-yukselen-yildizi.html



### LORAWAN Haberleşme Sistemi

LoRaWAN yani Long Range teknolojisi ile haberleşme yapan LoRa sensörleri ve lora kontrolörleri LoRa gateway cihazı ile kablosuz irtibatlamak suretiyle sahadan veri toplamak ve sahaya komut vermek için kullanılan sistemerdir.
Sahadan gelen tüm veriler LoRa gateway üzerinden bir LoRa IoT bulut platformuna gönderilir. Bu cloud platformu istenen analizleri yapar ve gerekirse sahaya otomtik olarak belli koşullara bağlı komutlar gönderebilir.
Örneğin seraların yer aldığı bir sahada, sera içindeki nem oranı düştüğünde, lora nem sensörü bu değeri LoRa geçit cihazı vasıtasıyla iot bulut platformuna iletir. Bu durum bulut platformunun sahadaki lora controller cihazını tetiklemesine yol açar ve kontroller su vanasını çalıştırır.
Ayrıca sahadaki modbus sistemler de LoRa kablosuz ağı üzerinden SCADA sistemine entegre edilebilir.



### LPWAN nedir

LPWAN (Low Power Wide Area Network), düşük güç tüketimi ile geniş alan kapsaması sağlayan bir kablosuz haberleşme teknolojisidir. LPWAN teknolojisi, genellikle nesnelerin interneti (IoT) uygulamaları için kullanılır ve düşük bant genişliğine sahip cihazların uzun mesafeler boyunca veri iletmesini sağlar

**LPWAN teknolojisinin popüler örnekleri şunlardır:**

- LoRaWAN: Uzun mesafelerde veri iletimi için kullanılan bir protokol olup, özellikle düşük güç tüketimi ve geniş kapsama alanı sunar

- NB-IoT (Narrowband IoT): Hücresel ağlarla entegre çalışan bir LPWAN teknolojisi olup, düşük veri hızları ve geniş kapsama alanı sunar.




### LoRa'nın Geleceği
LoRa teknolojisinin sınırlarının ve özelliklerinin doğru bir şekilde anlaşılması gerekliliğini göz önünde bulundurduğumuzda dahi, LoRa haberleşme teknolojisinin önümüzdeki süreçte çok büyük bir potansiyele sahip olduğunu göz ardı etmememiz gerekir. Henüz gelişmekte olan bir teknoloji olmasına karşın özellikle Hollanda’da ışıklandırma, akıllı tarım, atık takibi ve sayaç okuma uygulamalarındaki başarıları bu potansiyelin en büyük kanıtları olmuştur. Son dönemde haberleşme donanımı üreticilerinin LoRa destekli ürün portföyünde görülen çeşitlilik artışı da, LoRa’nın kablosuz haberleşme teknolojilerinin yıldızı olduğunun göstergelerinden bir başkasıdır. 

# KAYNAKÇA
- https://gsl.com.tr/lora-kablosuz-haberlesmenin-yukselen-yildizi.html
- https://kalitenetwork.com/blog/lora-ve-lorawan-nedir
- https://gelecekbt.com/lora
- https://blog.direnc.net/lora-ve-lorawan-nedir/
