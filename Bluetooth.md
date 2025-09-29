# Bluetooth Kablosuz Haberleşme 


**Bluetooth**, kısa menzilli kablosuz ses ve veri iletişimi için kullanılır. Bir Kablosuz Kişisel Alan Ağı (WPAN) teknolojisidir ve daha kısa mesafelerde veri iletişimi için kullanılır. Bu nesil, 1994 yılında Ericson tarafından icat edilmiştir. 2,4 GHz ile 2,485 GHz arasındaki lisanssız, ticari, bilimsel ve klinik (ISM) bantlarında çalışır. Bluetooth, 10 metreye kadar menzil sunar. Sürüme bağlı olarak en az 1 Mbps veya 3 Mbps'ye kadar veri sunar. Kullandığı yayma yöntemi **FHSS'dir (Frekans Atlamalı Açılım Spektrumu)**. Bir Bluetooth ağına pikonet, birbirine bağlı pikonet grubuna ise saçılım ağı denir.

---

## Frequency-Hopping Spread Spectrum in Wireless Networks (Kablosuz Ağlarda Frekans Atlamalı Yayılı Spektrum)

Frekans atlamalı yayılmış spektrum, farklı frekanslardaki kısa paketleri geniş kanal bant genişliği boyunca ileterek gürültülü ortamlarda sağlam bir şekilde çalışmak üzere tasarlanmıştır. Alıcı, bu "yakın" sinyalleri birbiriyle ilişkilendirir ve demodülasyon için en iyi sinyali seçer; bu da genellikle benzer koşullar altında çalışan frekans atlamasız alıcılara kıyasla daha iyi performans sağlar.

<img width="1078" height="389" alt="image" src="https://github.com/user-attachments/assets/d175de78-8673-4348-a176-aa2fe4cb3580" />

Yaygın spektrumlu iletimde (Spread Spectrum), veri kısa süreli kesintilerle farklı taşıyıcı frekanslar üzerinden iletilir. Frekans atlamalı yaygın spektrum (FHSS) sistemlerinde her bileşen farklı bir taşıyıcı frekansında gönderilir ve iletilen güç bir veya birkaç frekansa yoğunlaştırılır. Taşıyıcı frekansları, uzun vadede tahmin edilememesi için yarı rastgele bir sıralamaya göre değişir. Alıcı, sinyali gürültü ve girişimden etkilenmeyen dizilerle ilişkilendirir. FHSS uygulamalarında en yaygın dizi türleri Bluetooth ve IEEE 802.15.4’te kullanılan ikili ofset kodlarıdır. Sözde rastgele sayı üretecinin (PRNG) çıkışı, bir atlama kümesindeki frekans sayısına göre sayıcıya beslenir ve hem alıcı hem verici tarafında senkronize edilir. Bu yöntem, birden fazla paralel dizi kullanılarak sistemin dayanıklılığını artırabilir.

---

Bluetooth, telefon, tablet ve kulaklık gibi cihazların kablo gerektirmeden birbirine bağlanmasını ve bilgi paylaşmasını sağlayan kablosuz bir teknolojidir. Bluetooth, radyo dalgalarını kullanarak veri iletme ve alma prensibini temel alır . Bluetooth'u olan diğer cihazlarla eşleştirilebilir, ancak bağlantı kurmak için cihazın tahmini iletişim menzili içinde olması gerekir. İki cihaz veri paylaşmaya başladığında, beşten fazla cihazı barındırabilen piconet adı verilen bir ağ oluştururlar.

## Bluetooth'un Temel Özellikleri
Bluetooth’un iletim kapasitesi 720 kbps’dir.
Bluetooth kablosuz bir teknolojidir.
Bluetooth, düşük maliyetli ve kısa mesafeli bir radyo iletişim standardıdır.
Bluetooth sağlam ve esnektir.
Bluetooth'un temel mimari birimi **piconet**'tir .

---

## Bluetooth'un mimarisi

Bluetooth mimarisi iki tür ağ tanımlar: Piconet, Scatternet

### Piconet

Piconet, master node adı verilen bir birincil düğüm ve slave düğüm adı verilen yedi aktif ikincil düğüm içeren bir Bluetooth ağı türüdür . Dolayısıyla, 10 metre mesafede toplam 8 aktif düğüm olduğunu söyleyebiliriz. Birincil ve ikincil düğümler arasındaki iletişim one-to-one veya one-to-many olabilir. Mümkün olan iletişim yalnızca ana ve köle düğümler arasında gerçekleşir; Slave-slave iletişimi mümkün değildir. Ayrıca 255 adet park edilmiş düğümü vardır; bunlar ikincil düğümlerdir ve aktif duruma dönüştürülmedikçe iletişime katılamazlar.

<img width="614" height="476" alt="image" src="https://github.com/user-attachments/assets/3d45da9b-ae9d-4213-8c2a-e928c692548b" />




Resim kaynakçası -> https://www.geeksforgeeks.org/computer-networks/bluetooth/



### Scatternet

Çeşitli pikonetler kullanılarak oluşturulur. Bir pikonette bulunan bir slave node, başka bir pikonette master node veya birincil düğüm olarak görev yapabilir. Bu tür düğümler, bir pikonetteki master node'dan mesaj alabilir ve mesajı, master node olarak görev yaptığı diğer pikonetteki slave'ine iletebilir. Bu tür düğümlere köprü düğümü(bridge node) denir. Bir istasyon iki pikonette master node olarak kullanılamaz.


<img width="1040" height="436" alt="image" src="https://github.com/user-attachments/assets/fd10e6e0-8964-45a3-9d1c-b8f9dfeda55d" />



Resim kaynakçası -> https://www.geeksforgeeks.org/computer-networks/bluetooth/


---

## Bluetooth Protocol Stack (Bluetooth Protokol Yığını)

- **Radio (RF) Layer:** Frekans, frekans atlama kullanımı ve iletim gücü gibi hava arayüzünün ayrıntılarını belirler. Verilerin RF sinyallerine modülasyonunu/demodülasyonunu gerçekleştirir . Bluetooth alıcı-vericilerinin fiziksel özelliklerini tanımlar. İki tür fiziksel bağlantı tanımlar: bağlantısız ve bağlantı odaklı. 
- **Baseband Link Layer:** Temel bant, bir Bluetooth sisteminin dijital motorudur ve LAN'lardaki MAC alt katmanına eşdeğerdir. Bir piconet içinde bağlantı kurma, adresleme, paket formatı, zamanlama ve güç kontrolünü gerçekleştirir. 
- **Link Manager Protocol Layer:** Kimlik doğrulama ve şifreleme süreçlerini de içeren, halihazırda kurulmuş bağlantıların yönetimini gerçekleştirir. Bağlantıları oluşturmaktan, sağlıklarını izlemekten ve komut veya başarısızlık durumunda bunları sorunsuz bir şekilde sonlandırmaktan sorumludur. 
- **Logical Link Control and Adaption (L2CAP) Protocol Layer:** Bluetooth protokol yığınının kalbi olarak da bilinir. Bluetooth protokol yığınının üst ve alt katmanları arasında iletişime olanak tanır. Üst katmanlardan alınan veri paketlerini alt katmanların beklediği biçimde paketler. Ayrıca segmentasyon ve çoklama işlemlerini gerçekleştirir.
- **Service Discovery Protocol (SDP) Layer:** Hizmet Keşif Protokolü'nün kısaltmasıdır. Bluetooth özellikli başka bir cihazda mevcut hizmetleri keşfetmenizi sağlar.  
- **RF Comm Layer:** Bir kablo değiştirme protokolüdür. Radyo Ön Uç Bileşeni'nin kısaltmasıdır. WAP ve OBEX ile seri arayüz sağlar. Ayrıca, mantıksal bağlantı kontrol ve uyarlama protokolü (L2CAP) üzerinden seri portların emülasyonunu da sağlar. Protokol, ETSI standardı TS 07.10'a dayanmaktadır.
- **OBEX:** Object Exchange'in kısaltmasıdır. 2 cihaz arasında nesne alışverişi yapmak için kullanılan bir iletişim protokolüdür. 
- **WAP:** Kablosuz Erişim Protokolü'nün kısaltmasıdır. İnternet erişimi için kullanılır.
- **TCS:** Telephony Control Protocol'ün  kısaltmasıdır . Telefon hizmeti sağlar. Bu katmanın temel işlevi, birden fazla cihaza hizmet veren ağ geçidi için çağrı kontrolü (kurulum ve iptal) ve grup yönetimidir.
- **Application Layer:** Kullanıcının uygulama ile etkileşime girmesini sağlar.



<img width="1019" height="668" alt="image" src="https://github.com/user-attachments/assets/61241553-2236-472a-b7d8-621218a8d276" />


---

## Bluetooth Türleri

- **Araç İçi Kulaklık:** Cep telefonu kullanmadan araç hoparlör sisteminden arama yapılabilir.
- **Stereo Kulaklık:** Arabada veya evdeki müzik çalarlarda müzik dinlemek için.
- **Webcam:** Bluetooth yardımıyla kamerayı dizüstü bilgisayarınıza veya telefonunuza bağlayabilirsiniz.
- **Bluetooth Bağlantılı Yazıcı:** Yazıcı, cep telefonu veya dizüstü bilgisayara Bluetooth aracılığıyla bağlandığında kullanılabilir.
- **Bluetooth Küresel Konumlandırma Sistemi (GPS(Global Positioning System)):** Arabalarda Küresel Konumlandırma Sistemi'ni (GPS) kullanmak için , kişinin telefonunu Bluetooth aracılığıyla araç sistemine bağlaması ve adresin yönünü alması gerekir.


---

## Bluetooth'un uygulamaları


- Kablosuz kulaklıklarda, kablosuz PAN'larda ve LAN'larda kullanılabilir .
- Dijital kamerayı kablosuz olarak cep telefonuna bağlayabilir.
- Video, şarkı, fotoğraf veya dosya anlamındaki verileri bir cep telefonundan başka bir cep telefonuna veya bilgisayara aktarabilir.
- Tıbbi sağlık, spor ve fitness, askeri sektörlerde kullanılmaktadır.



## Avantajları
- Düşük maliyetli ve kullanımı kolay bir cihazdır.
- Duvarlardan da geçebilir.
- Hiçbir kabloya ihtiyaç duymadan anında Ad-hoc bağlantı oluşturur .
- Ses ve veri aktarımında kullanılır.


## Dezavantajları
- Hacklenebilir ve bu nedenle daha az güvenlidir.
- 3 Mbps gibi yavaş bir veri aktarım hızına sahiptir.
- Bluetooth iletişimi yönlendirmeyi desteklemiyor .

---

# Bizim Projemiz

## Amacımız
Bluetooth cihazlarının menzilini artırmak için LoRa’yı bir köprü (bridge) olarak kullanmak

## Mantık ve Temel Prensip

Bluetooth cihazları genellikle 10–100 metre arasında çalışır (Bluetooth Classic ve BLE farkları var). LoRa ise kilometrelerce menzile çıkabilir (şehir içi 2–5 km, açık alan 10–15 km).

**Bizim sistemimiz şu şekilde çalışacak:**

- Bir cihazın Bluetooth verisi Raspberry Pi’ye gelir.

- Raspberry Pi, bu veriyi LoRa modülü üzerinden gönderir.

- Karşı tarafta başka bir LoRa modülü bu veriyi alır.

- Karşı tarafın Raspberry Pi’si tekrar veriyi Bluetooth cihazına iletir.

Yani aslında Bluetooth + LoRa köprüsü kuruyoruz. Bluetooth kısa mesafeli, LoRa uzun mesafeli.

Bu sistem aslında **“Bluetooth Mesh / Long Range Gateway”** gibi düşünülebilir.


**LoRa çok yavaş(genellikle 0.3–50 kbps), bluetooth üzerinden yüksek veri aktarırsak çok yavaş oluyor. LoRa paket bazlı çalışır. Eğer sürekli ve hızlı veri akışı istersen gecikmeler olabilir. Bluetooth verisini direkt LoRa’ya gönderemeyiz, onu bir protokole (örneğin seri veri) çevirmemiz gerekir. Yani LoRa “tünel” gibi çalışacak.**


### Kısaca 

- **Bluetooth**: kısa mesafe, düşük güç, cihaz eşleştirme.

- **LoRa**: uzun mesafe, düşük veri hızı, tek yönlü veya çift yönlü veri aktarımı.

- **Raspberry Pi**: veri alıcı, protokol çevirici, köprü.


---
### Şema gösterimi

<img width="1198" height="583" alt="image" src="https://github.com/user-attachments/assets/df3dc915-e77f-4ddc-b189-4fdb015db8cf" />


---

## Bluetooth C# Kodu

Bluetooth üzerinden C# ile kablosuz iletişim kurmak istiyorsanız, temel olarak iki yaklaşım vardır:

- Windows’un yerleşik Bluetooth API’lerini kullanmak (Windows.Devices.Bluetooth namespace’i).

- Üçüncü taraf kütüphaneler kullanmak (32feet.NET)

**En yaygın ve pratik yöntem genellikle 32feet.NET kütüphanesidir. Bu kütüphane, hem klasik Bluetooth hem de RFCOMM (seri port emülasyonu) üzerinden cihazlarla iletişim kurmayı kolaylaştırır.**

### Classic Bluetooth (RFCOMM / SPP)
```charp
dotnet add package InTheHand.Net.Bluetooth
```

### BLE (GATT)
```charp
dotnet add package InTheHand.BluetoothLE
```



### Bluetooth Cihazlarını Listeleme


```charp
using System;
using System.Linq;
using System.Text;
using InTheHand.Net.Sockets;
using InTheHand.Net.Bluetooth;

class Program
{
    static void Main()
    {
        Console.WriteLine("Cihazlar aranıyor...");
        using var cli = new BluetoothClient();
        var devices = cli.DiscoverDevices(); // IReadOnlyCollection<BluetoothDeviceInfo>

        if (devices == null || devices.Count == 0)
        {
            Console.WriteLine("Hiç cihaz bulunamadı.");
            return;
        }

        int i = 0;
        foreach (var d in devices)
        {
            Console.WriteLine($"{i}: {d.DeviceName} - {d.DeviceAddress}");
            i++;
        }

        Console.Write("Bağlanmak için index gir: ");
        if (!int.TryParse(Console.ReadLine(), out int idx) || idx < 0 || idx >= devices.Count)
        {
            Console.WriteLine("Geçersiz index.");
            return;
        }

        var device = devices.ElementAt(idx); // ElementAt için System.Linq gerekli
        Console.WriteLine($"Seçildi: {device.DeviceName} - {device.DeviceAddress}");

        try
        {
            cli.Connect(device.DeviceAddress, BluetoothService.SerialPort);
            using var stream = cli.GetStream();
            var data = Encoding.ASCII.GetBytes("Merhaba Bluetooth!");
            stream.Write(data, 0, data.Length);
            Console.WriteLine("Mesaj gönderildi.");
        }
        catch (Exception ex)
        {
            Console.WriteLine("Bağlantı hatası: " + ex.Message);
        }
    }
}
```


### Bluetooth’a Bağlanma ve Veri Gönderme (Raspberry'e bağlanırken bu kodu çalıştırabiliriz)

```charp
using System;
using System.Linq;
using System.Text;
using InTheHand.Net.Sockets;
using InTheHand.Net.Bluetooth;

class Program
{
    static void Main()
    {
        Console.WriteLine("Cihazlar aranıyor...");
        using var cli = new BluetoothClient();
        var devices = cli.DiscoverDevices().ToList();

        if (devices.Count == 0)
        {
            Console.WriteLine("Hiç cihaz bulunamadı.");
            return;
        }

        for (int i = 0; i < devices.Count; i++)
        {
            Console.WriteLine($"{i}: {devices[i].DeviceName} - {devices[i].DeviceAddress}");
        }

        Console.Write("Bağlanmak için index gir: ");
        if (!int.TryParse(Console.ReadLine(), out int idx) || idx < 0 || idx >= devices.Count)
        {
            Console.WriteLine("Geçersiz index.");
            return;
        }

        var device = devices[idx];
        Console.WriteLine($"Seçildi: {device.DeviceName} - {device.DeviceAddress}");

        try
        {
            // SPP servisine bağlan
            cli.Connect(device.DeviceAddress, BluetoothService.SerialPort);
            Console.WriteLine("Bağlantı başarılı!");

            using var stream = cli.GetStream();

            // Mesaj gönder
            string mesaj = "Merhaba Bluetooth!";
            byte[] data = Encoding.ASCII.GetBytes(mesaj);
            stream.Write(data, 0, data.Length);
            Console.WriteLine($"Mesaj gönderildi: {mesaj}");

            // İstersen karşı taraftan cevap oku
            byte[] buffer = new byte[256];
            int bytesRead = stream.Read(buffer, 0, buffer.Length);
            if (bytesRead > 0)
            {
                string cevap = Encoding.ASCII.GetString(buffer, 0, bytesRead);
                Console.WriteLine($"Cevap alındı: {cevap}");
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Bağlantı hatası: " + ex.Message);
        }
    }
}
```




### Raspberry Pi Tarafında Bluetooth Mesajını Yakalama

Bizim C# kodumuzun gönderdiği "Merhaba Bluetooth!" mesajı, Raspberry Pi’ye seri port üzerinden düşecek (/dev/rfcomm0).
Pi tarafında bu mesajı yakalayıp LoRa’ya aktarmamız lazım.


```charp
using System;
using System.IO.Ports;

class SenderBridge
{
    static void Main()
    {
        // Bluetooth seri portu (RFCOMM bağlanınca oluşur)
        var bt = new SerialPort("/dev/rfcomm0", 9600);
        // LoRa seri portu (UART'a bağlı modül)
        var lora = new SerialPort("/dev/serial0", 9600);

        bt.Open();
        lora.Open();

        Console.WriteLine("Bluetooth → LoRa köprüsü başlatıldı...");

        while (true)
        {
            try
            {
                string line = bt.ReadLine(); // Bluetooth’tan oku
                if (!string.IsNullOrWhiteSpace(line))
                {
                    Console.WriteLine("Bluetooth’tan geldi: " + line);
                    lora.WriteLine(line); // LoRa’ya aktar
                    Console.WriteLine("LoRa’ya gönderildi.");
                }
            }
            catch (TimeoutException) { }
        }
    }
}
```


### Karşı Taraftaki Raspberry Pi (LoRa Alıcı)

Bu Pi, LoRa’dan gelen veriyi okuyup Bluetooth üzerinden çıkış yapacak.

```charp
using System;
using System.IO.Ports;

class ReceiverBridge
{
    static void Main()
    {
        var lora = new SerialPort("/dev/serial0", 9600);
        var bt   = new SerialPort("/dev/rfcomm0", 9600);

        lora.Open();
        bt.Open();

        Console.WriteLine("LoRa → Bluetooth köprüsü başlatıldı...");

        while (true)
        {
            try
            {
                string line = lora.ReadLine(); // LoRa’dan oku
                if (!string.IsNullOrWhiteSpace(line))
                {
                    Console.WriteLine("LoRa’dan geldi: " + line);
                    bt.WriteLine(line); // Bluetooth’a aktar
                    Console.WriteLine("Bluetooth’a gönderildi.");
                }
            }
            catch (TimeoutException) { }
        }
    }
}
```




**LoRa modülünün pi'ye UART üzerinden bağlı olması gerekiyor. Olduğu portu da kodda belirtmemiz lazım**



# KAYNAKÇA
- https://www.geeksforgeeks.org/computer-networks/bluetooth/
- https://electronics.howstuffworks.com/bluetooth.htm
- https://www.sony.co.uk/electronics/support/articles/00030769
- https://www.cisa.gov/news-events/news/understanding-bluetooth-technology
- https://www.7signal.com/bluetooth
