## NETWORK Notlarım

Bu repository [Sistem ve Network Mühendisliği](https://www.udemy.com/course/sistem-ve-network-muhendisligi/) eğitimi alırken tutmuş olduğum notlardan oluşmaktadır.

# İçerik Tablosu

* [AĞ TEMELLERİ (Network Basics)](#AĞ-TEMELLERİ-Network-Basics)

* [TEMEL AĞ DONANIMLARI (Basic Network Devices)](#TEMEL-AĞ-DONANIMLARI-Basic-Network-Devices)

* [AĞ KABLOLARI (NETWORK CABLES)](#AĞ-KABLOLARI-NETWORK-CABLES)

* [AĞ MİMARİLERİ VE PROTOKOLLERİ (Network Architectures and Protocols)](#AĞ-MİMARİLERİ-VE-PROTOKOLLERİ-Network-Architectures-and-Protocols)

* [IP ADRESLERİ](#IP-ADRESLERİ)

* [AĞ SERVİSLERİ (NETWORK SERVICES)](#AĞ-SERVİSLERİ-NETWORK-SERVICES)

## AĞ TEMELLERİ (Network Basics)

### Ağ (Network)

* Birbirleri ile belirli kurallar çerçevesinde iletişim kurabilen cihazların oluşturduğu yapıdır.

#### Ağ Sistemlerinin Yararları

* **Program Paylaşımı:** Bir ağ ortamında tüm kullanıcılar merkezi bir bilgisayara kurulmuş olan programı kullanabilirler.

* **Dosya Paylaşımı:** Kullanıcılar, işlerini yaparken kullandıkları dosya kaynaklarını ağdaki diğer bilgisayarlardan, izinler dahilinde elde edebilirler.

* **Yazıcı Paylaşımı:** Ağdaki birçok kullanıcı ortak bir yazıcıyı kullanabilirler. Maliyet açısından önemlidir.

* **Güvenlik:** Bir ağa bağlanıp kaynakları kullanmak isteyenlerin kimlik doğrulaması gerekir. Ve ağdaki kaynakları yetkileri dahilinde kullanabilirler.

* **Merkezi Yönetim:** Bir ağdaki tüm cihazlar ve bilgisayarlar, sistem yöneticileri tarafından uzaktan yönetilebilirler.

### Ağ Bileşenleri
 * Yazılım ve donanımlardan oluşur.
    - **Yazılım;** işletim sistemleri, iletişim protokolleri ve ağ programlarından oluşur.

    - **Donanım;** kablo, switch, router, bilgisayar, NIC gibi donanımlarından oluşur.

* Ağ ortamında çalışabilen işletim sistemleri 2 farklı rol üstlenirler.

    - 1) **Sunucu (Server):** Ağ kaynaklarını elinde tutan ve diğer bilgisayarlara yetkiler dahilinde sunan işletim sistemleridir. Örn; Windows Server 2016

    - 2) **İstemci (Client):** Sunulan kaynaklara erişebilen işletim sistemleridir. Örn; Windows 10

### Ağ Cihazları (Network Devices)

* Bir ağı oluşturmak için kablo, kart ve bilgisayar yeterlidir. Fakat ağ genişlemeye başladığında bir takım cihazların da yardımı gerekir. Örneğin;

    - 10 bilgisayarı birbirine bağlamak için her bir bilgisayara 10 kart (veya 4 portlu 5 kart) takılması gerekir. Bu mümkün olamaz. 
    - Veya bu 10 bilgisayardan biri bile 500 metre uzaklıkta ise sinyal taşımak mümkün olamaz.

* Bu cihazlar ağa mesafe, performans, güvenlik gibi özellikler katarlar.

## TEMEL AĞ DONANIMLARI (Basic Network Devices)

* Ağa bağlanmak isteyen her cihaz ve bilgisayarda olması zorunlu bir donanımdır.

* Ağa gönderilecek olan veriyi elektrik sinyaline dönüştürür ve kabloya iletir.

* Sayısal-mantıksal çevrimler, başarım kontrolü, performans yönetimi gibi özelliklere sahiptir.

* ISA ve PCI slotlarına takılabilirler.

* Günümüzde anakarta tümleşik (On-Board) de üretilirler.

* Hızları, teknolojileri ve kablo tipine bağlıdır.

* Kullanılan kablo cinsleri için farklı konnektör tiplerine sahiptir.

* Ethernet NIC’ler hızlarına göre 10 Mbps (Ethernet), 100 Mbps (FastEthernet), 1 Gbps (Gigabit Etrhernet), 10 Gbps (10GigabitEthernet) olarak 4 seviyeye ayrılırlar. *Ethernet ile NIC, ayrı terimlerdir. NIC, etherneti kapsar.

### Repeater (Tekrarlayıcı) ve Hub (Merkez)

* Ağda kullanılan kabloların maksimum erişim mesafeleri vardır.

    - Örneğin UTP kablo, sinyali max 100 metre mesafeye taşıyabilir. Daha uzak mesafeye taşınabilmesi için araya Repeater veya Hub konulması gerekir.

* Repeater veya Hub , azalan sinyal gücünü yükselterek daha uzak mesafeye veri iletimini sağlarlar.

    - Repeater, tek portlu; Hub, çok portludur

    - Bu, kablosuz yayınlar için de geçerlidir.

### Ağ Anahtarı (Network Switch)

* Bilgisayar ve diğer ağ donanımlarının birbirilerine bağlanmasını sağlarlar.

* Hub ve Repeater’lardan farklı olarak, kendisine bağlı olan cihazların MAC adreslerini bilmesi ve iletişimi bu MAC adreslerine göre adreslemesi/anahtarlamasıdır.

* OSI ve TCP/IP katmanlarının (Layers) 2 veya 3.sünde çalışır.

* L3 switchlerde IP Routing, Port Mirroring, VLAN, Port-MAC Matching gibi teknolojiler bulunmaktadır.

* Switchler komut arayüzü (CLI) veya web arayüzü (HTTP) üzerinden konfigüre edilebilir.

* Birbirilerine de bağlanabilirler. Birbirilerine bağlı oldukları porta Uplink Port adı verilir.

### Yönlendirici (Router)

* Geniş ağlarda ve internette kullanılırlar.

* Sadece MAC adreslerine göre değil; IP adreslerine göre de yönlendirme yaparlar.

* Yapısı birbirinden farklı networkleri haberleştirirler. 

* Verileri bir ağdan diğerine yönlendirirler.

* Kendisine gelen veriyi, hedefe en kısa yoldan erişitirme hesaplamaları yaparlar.

* Yazılımsal olarak da bu rolü temel düzeyde üstlenmiş farklı cihazlar vardır.

### Modem (Modem)

* Modulator-demodulator kelimelerinin ilk kısımlarından türetilen bir terimdir.

* Analog-Dijital ve Dijital-Dijitaldönüşüm yapan 2 tiptedir.

* Ethernet kartından gönderilen veriyi, internet sağlayıcıdan kiralanan hattın türüne göre dönüşüm yapar.

* Ethernet sinyallerini xDSL, PSTN, ISDN veya Kabla hattı üzerinde hareket edecek yapıya dönüştürür.

* Eğer hat dijital ise Dijital-Dijital; analog ise Dijital-Analog dönüşümü yapar.

### Güvenlik Duvarı (Firewall)

* Yazılımsal ve donaımsal olarak 2 tiptir.

* İç ve dış ağ arasında gelen-giden verilerin (paketlerin) kontrolünü yapar. Zararlı verileri ve siber tehditleri bloklar.

* Sistem yöneticisi tarafından yapılandırılması gerekir.

* Zaafiyet göstermemesi için doğru yapılandırılması önemlidir.

* Web arayüzü veya komut arayüzü (CLI) ile yapılandılabilir.

* Birden çok güvenlik önlemi özellikli firewall’lar, UTM(Unified Threat Management) firewall’dur.

* Router gibi de davaranabilir; verilerin (paketlerin) yönlendirilmesini sağlayabilir.

* Yazılımsal firewall’lar işletim sistemleri üzerine uygulama olarak kurulabilirler.

## AĞ KABLOLARI (NETWORK CABLES)

* Bir yerel ağda, bilgisayarlar ile switch arasında ve telefon bağlantılarında kullanılabilirler.

* Birbirilerine ikili (pair) olarak sarılmış kablolardan oluşurlar.

* 100 metre mesafeye kadar sinyal taşıyabilirler. 

* RJ45 jack kullanılarlar. Ve tip olarak ikiye ayrılırlar.

    1) **Unshielded Twisted Pair (UTP):**
    Pair’lerin etrafında koruyucu yoktur. Elektromanyetik alandan etkilenirler. Daha esnek oldukları için tercih edilirler.
    
    2) **Sheilded Twisted Pair (STP):**
    Hem pair’lerin hem de kablonun etrafı metal bir koruyucu ile sarılıdır. Elektromanyetik alandan etkilenmezler.

### Twisted Pair Kablolar

* Kategori olarak 8’e ayrılırlar

    1) Cat1: Telefon hatlarında kullanılmışlardır. 
    
    2) Cat2: 4 Mbps Token Ring ağlarında kullanılmışlardır. 

    3) Cat3: 10 Mbps ethernet ağlarında kullanılmışlardır.

    4) Cat4: 16 Mbps ethernet ağlarında kullanılmışlardır. 
    
    5) Cat5: 4 pair’den oluşur. 1 Gbps ethernet ağlarında kullanılabilirler. RJ45 konnektörler ile bağlanırlar.

    6) Cat5e: 4 pair’den oluşur. 1 Gbps ethernet ağlarında kullanılırlar. Cat5’e göre Crosstalk daha az gerçekleşir.

    7) Cat6: 4 pair’den oluşur. 1 Gbps ağlarda kullanılır. 10 Gbps ağlarında da çalışabilir. Cat5 ve Cat5e’ye göre Crosstalk çok daha düşüktür. 8P8C konnektör ile bağlanırlar. RJ45 ile aynı görünümdedir.

    8) Cat7: 4 pair’den oluşur. Crosstalk’u önlemek için kalkan kullanılır. 10 Gbps ağlar için üretilmişlerdir.

* Bağlantı tipi olarak 2’ye ayrılırlar.

    1) **Düz (Straight) Kablo:**
    - Kablonun her iki ucu aynı renk sırasına göre bağlanır.
        
    - Bilgisayar-switch, switch-router gibi farklı kategori cihazlar içindir.
        
    - İki farklı renk sırasına göre sıralanabilir.

        a) 568A: 1-YB  2-Y 3-TB  4-M 5-MB  6-T 7-KB  8-K 
        
        b) 568B: 1-TB  2-T 3-YB  4-M 5-MB  6-Y 7-KB  8-K

    2) **Çapraz (Crossover) Kablo:**

    - Kablonun her iki ucu farklı renk sırasına göre bağlanır.
 
    - Bilgisayar-bilgisayar, switch-switch gibi aynı kategori cihazlar içindir. 

    - RJ45’teki 8 pinden sadece 1, 2, 3 ve 6. pin kullanılır. 

    - 1 ve 2. pin veri göndermek için; 3 ve 6. pin veri almak içindir. 

    - Bir ucu 568A, diğer ucu 568B olarak bağlanmalıdır.
 
    - 100 Mbps hız alınır.
 
    - Artık cihaz NIC’leri düz-çapraz ayrımını kendi içlerinde yapabildikleri için gerek kalmamıştır.

### Fiber Optik Kablolar

* Veri iletimini cam ya da plastik fiber üzerinden ışık sinyalleri ile sağlarlar. 

* Sinyalin dışarı yansımasını önleyici katmanlar (kılıflar) vardır.

* Işık sinyali, elektromanyetikten etkilenmez. 

* Sinyal, en içteki core adı verilen katmanda ilerler. 

* Bakır kablolardan çok daha uzak mesafelere veri iletebilirler. 

* Bağlantı tipi olarak 2’ye ayrılırlar.
    1) **Single Mode Fiber Kablo:**
    
    - Core tabaka incedir. 

    - Aynı anda 1 ve tek yönlü ışık sinyali taşıyabilir.
 
    - 100 km’ye kadar veri iletebilir. 

    - Işık kaynağı lazerdir.

    - Bağlantı konnektörü olarak Straight Tip (ST) kullanılır.
 
    2) **Multi Mode Fiber Kablo:**

    - Core tabaka kalındır. 

    - Aynı anda birçok ışık sinyali taşıyabilir. 

    - 2 km’ye kadar veri iletebilir. 

    - Işık kaynağı LED’dir. 

    - Bağlantı konnektörü olarak Subscriber Connector (SC) kullanılır.

## AĞ MİMARİLERİ VE PROTOKOLLERİ (Network Architectures and Protocols)

### Ağ Mimarisi

* Bir ağın mimairisini belirleyen 2 temel özellik vardır.
    1) **Ağ Topolojisi:** Cihazların kablo ve bağlantı yerleşim haritası gibi düşünülebilir.

        A) **Bus Topoloji:** Bütün cihazları birbirine bağlamak için hepsine uğrayan doğrusal bir kablo ile sağlanır.

        B) **Star Topoloji:** Bilgisayarların swtich, router gibi cihazlar ile birbirine bağlandıkları yapıdır.

        C) **Ring Topoloji:** Fiziksel olarak Star’a benzer ama mantıksal olarak Ring’tir. Veriler ağ üzerinde halka şeklinde bir döngüye sahiptir.

    2) Ağın Büyüklüğü: Ağlar, büyüklüklerine göre 2’ye ayrılırlar.

        A) **LAN (Local Area Network):** LAN’lar yüksek hızlı, güvenilir ve küçük bir alana yayılmış olan lokal ağlardır. Örn; bir şirketin içindeki ağdır.

        B) **WAN (Wide Area Network):** Coğrafi olarak birbirinden uzak LAN’ların birleştirilmesiyle oluşan ağdır. Örn; internet ağı.

        - İpucu: Bir daire LAN ise; apartman WAN’dır. 

        - Bir apartman LAN ise; site WAN’dır.
    
### WAN Terminolojisi

*	**Toll Network:** Servis sağlayıcısına ait ağ bulutudur. 

*	**POP (Point of Presence):** Servis sağlayıcının cihazlarının bulunduğu noktadır. 

*	**CPE (Costumer Premises Equipment):** Servis sağlayıcının, kullanıcıların binalarında bulundurduğu cihazdır. 

* **Local Loop:** POP’tan servis sağlayıcının merkezine yapılan kablolamadır. 

*	**CO Switch:** Kullanacıya hizmet sağlayan en yakın switch’lerdir. 

*	**Demarcation:** CPE’nin bittiği ve Local Loop’un başladığı noktadır. 

*	**ISP (Internet Service Provider):** İnternet servis hizmeti sağlayıcısıdır.

### Ağ Protokolü

* Ağda çalışan cihazların iletişim kurabilmeleri için gerekli kurallar bütünüdür.

* Ağ protokollerini dillere benzetebiliriz. İnsanların anlaşabilmesi gibi bilgisayarların da aynı protokolleri kullanıp anlaşabilmeleri gerekir.

* Günümüzde en yaygın kullanılan protokol TCP/IP (Transmission Control Protocol/Internet Protocol)’dir. TCP/IP her türlü ağda kullanılabilen esnek, gelişmiş ve hızlı bir protokoldür.

* Kullanılmak istenen protokolü, işletim sistemleri sağlar.

### OSI (Open Systems Interconnection) Referans Modeli

* Network iletişiminde ortak bir dil olarak 1984 yılında kullanılmaya başlanmıştır. 

* 7 katmandan oluşur. 

* Her bir katman, alt katmandan hizmet alır; üst katmana hizmet verir. 

* Gönderici her bir katmanda veriye (pakete) kendi bilgisini ekler. Alıcı da çıkarır. 

* Ekleme işlemine enkapsülasyon; çıkarma işlemine de deenkapsülasyon adı verilir.

    7- Application Layer (Uygulama Katmanı) 

    6- Presentation Layer  (Sunum Katmanı)

    5- Session Layer  (Oturum Katmanı)

    4- Transport Layer  (Ulaşım Katmanı)

    3- Network Layer  (Ağ Katmanı)

    2- Data-Link Layer  (Veri Bağlantı Katmanı)

    1- Physical Layer  (Fiziksel Katman)

### OSI (Open Systems Interconnection) Referans Modeli

#### 7- Application Layer (Uygulama Katmanı):

* E-posta, dosya transferi, web erişimi gibi ağ hizmetleri sağlayan servisleri destekler.

* Kullanıcının Google.com’u çağırdığını Presentation katmanına bildirir sadece.

* Presentation katmanından gelen paketi de uygulamada açıp kullanıcıya görüntüler.

* Gerisiyle ilgilenmez.

* Kullanıcıya en yakın, kullanıcı dostu katmandır. Kullanıcının bilgisayar dili tercümanı gibidir.

#### 6- Presentation Layer (Sunum Katmanı):

* Application katmanından gelen kullanıcının isteklerini yorumlayıp, alt katmanlara hazırlanması için işe koyulur.

* Dönüştürme işlemlerini yapar.

* Şifreleme, çözme; sıkıştırma, karakter seti değişimi, grafik komutlarının yorumlanması gibi işler burada yapılır.

* Gelen paketlerin kullanıcıya sunumu için de, burada hazırlanılır.

#### 5- Session Layer (Oturum Katmanı):

* Diğer bilgisayarlar ile iletişim sağlandığında uygulamalar arasında oturum burada açılır.

* Karşılıklı iki uygulamanın birbirini bulduğu katmandır.

* Bu oturumun kopmaması, stabil olması, oturumda veri senkronizasyonu gibi görevleri vardır. Çakışmaları önler.

* İletişimde problem olması halinde gönderilen verinin baştan komple gönderilmemesi için veriye checkpoint’ler koyar. Aksaklık halinde ne kadarı gönderilmediği tespit edilerek sadece o kısım gönderilir.

#### 4- Transport Layer (Ulaşım Katmanı):

* Birincil görevi, paketin alıcıya ulaştığından emin olmaktır.

* Session katmanından gelen verileri, network katmanın daha iyi anlayabileceği şekilde küçük parçalara böler.

* Bu parçalara segment adı verilir. Segment’leme görevi buranındır.

* Alt ve üst katmanların eş zamanlı çalışabilmesini de sağlar. Bu işleme multiplexing adı verilir.

* Web’de gezerken aynı anda download yapılabilmesinden bu katman sorumludur.

* TCP (Transmission Control Protocol) ve UDP (User Datagram Protocol) bu katmanda işlenir.

#### 3- Network Layer (Ağ Katmanı):

* En önemli katmandır.

* Paketlerin hangi route (rota) üzerinden gideceğini belirler.

* Paketin hedefe ulaşımında birden fazla rota varsa doğrusuna karar vermekle sorumludur.

* Bu yüzden IP adresi burada girilir.

* Verinin kalitesi (QoS – Quality of Service) de burada belirlenir.

* Segment boyutlarını, Data-Link katmanının daha iyi anlayabileceği daha küçük segmentlere böler.

#### 2- Data-Link (Veri Bağlantı Katmanı):

* Gönderilen verilerin elektrik sinyallerine dönüştürülüp kabloya iletilmesini ve tersi yöndeki işlemi gerçekleştiren katmandır.

* MAC bilgisi burada girilir.

* Network katmanından gelen segment’leri, Physical katmanda yola çıkabilecek şekilde frame’lere böler.

* Frame tipi gibi bilgiler burada eklenir.

* Yolda bozulabilecek frame’leri tespit etmek için frame’lere CRC (Cyclic Redundancy Check) bilgileri ekler.

* Karşı bilgisayarda CRC bilgisi doğru okunuyorsa frame bozulmamıştır.

#### 1- Physical Layer (Fiziksel Katman):

* Elektriksel, optik veya kablosuz sinyalleri A noktasından B noktasına iletmekle sorumludur. 

* Sadece bit’lerin bir bilgisayardan diğerine ulaşmasıyla ilgilenir.

* Paketi teslim etmekle sorumludur, içeriğiyle ilgilenmez.

* Bu katmanda pakete, paketin hangi sinyalle taşınacağı, bit’lerin ne şekilde dizileceği, konnektörlerdeki kaç pin ile çalışılacağı, adaptörün ne zaman veri gönderip alacağı, teslimatın başarı durumu gibi detaylar tanımlanır, pakete yazılır.

* Fiziksel detaylar…

### TCP (Transmission Control Protocol)

* Bağlantı temelli, güvenilir bir iletim protokolüdür. 

* Veri iletimine başlamadan önce gönderici ve alıcı arasında anlaşma sağlar. 

* Alıcıya ulaşmayan veriyi tekrar yollar.

### UDP (User Datagram Protocol)

* Bağlantı temelli değildir ve kontrol mekanizmaları içermez. 

* Kontroller yapmadığı için TCP’den hızlıdır. 

* Hızın, güvenirlikten önemli olduğu bağlantılarda kullanılır.

### Portlar (Ports)

* Portlar, bilgisayarların giriş kapılarıdırlar. 

* TCP ve UDP bağlantılar, veriyi üst katmanlara taşımak veya uygulamaya iletmek için port numaraları kullanırlar. 

* Port numaraları, aynı anda yapılan farklı iletişimleri ayırt etmek için kullanılırlar. 

* Her application katmanı servisi, belirli bir port’tan sunulur. 

* Bir bilgisayarda 65536 adet port vardır. 1024 tanesi iyi bilenendir. (Well-Known)

### TCP Bağlantı Başarım Araçları

#### ARP (Address Resolution Protocol):

* Ağ cihazlarının 2 adresi vardır.
    
    a)	**MAC:** 
    - Fiziksel adresidir. 
    - Ağ kartlarının ROM belleğine üreticisi tarafından yazılır. 
    - 48 bit’lik hexadecimal (on altılık) bir sayıdır. 
    Örn;  4F-00-1C-25-1B-4B
    
    b)	**IP:**	
    - Mantıksal adresidir. 
    - Cihazlara yöneticiler tarafından yazılır. 
    - 32 bit’lik binary (ikilik) bir sayıdır. 
    - Örn; 11000000.10101000.00000001.00001010 
    - Böyle bir sayıyı hatırlamak ve yazmak zor olduğu için her 8’li grup decimal’e (ondalık) çevrilmiştir. Sayı artık 192.168.1.10’dur.

### TCP Bağlantı Başarım Araçları

#### ICMP (Internet Control Message Protocol):

* Sorun gidermek ve hata tespiti için kullanılır.

    a) **Ping:** Kaynaktan hedefin IP’sine gönderilen 32 bit’lik küçük bir mesajdır (Echo    Request). Mesajı alan bilgisayar cevap verir (Echo Reply). Mesajın hedefe ulaşması zamanlarını da gösterir (Rount Trip Time).

    b) **Tracert:** Kaynaktan hedef IP’ye giderken geçilen IP ve cevap verme sürelerini gösterir. Yol (rota-route) üzerindeki her bir IP’ye hop adı verilir.

### IP (Internet Protocol) Adresi

* IP adresleri, cihazların network’teki yerlerini belirtir. Hangi ağda olduğunu ve ağdaki kimliğini belirtir.

* IP adresleri 32 bit’lik, binary ve mantıksal bir sayıdır.

* Örn; 11000000101010000000000100001010

    - Böyle bir sayıyı hatırlamak ve yazmak zor olduğu için önce 4 parçaya bölünür. 11000000.10101000.00000001.00001010 Her bir parçaya ‘octet’ adı verilir. Her IP’de 4 octet vardır.

    - Her octet de decimal’e (ondalık’a) çevrilir. IP artık bizler için 192.168.1.10 şeklindedir. Bilgisayar için hala en başındaki gibi binary’dir (ikilik’tir.)

* Bu kolaylık sağladığımız işleme ‘Dotted Decimal’ adı verilir.

* Her octet minimum 0; maksimum 255 değeri alabilir.

## IP ADRESLERİ

### IP (Internet Protocol) Adresi

* IP adresleri 2 kısımdan oluşur.

    1) **Network ID:** Network’ün kendine ait ID’sidir. Bu ID, cihazların hangi ağda olduğunu belirtir. Aynı ağda olan cihazların Network ID’leri aynı olmak zorundadır. Binary (ikilik)’de 1’lik bitlerin ard arda diziliminden oluşur. Araya 0 giremez.
    
    2) **Host ID:** Cihazın, ağda kendisini tanımlayan ID’dir. Aynı ağda olan cihazların Host ID’leri farklı olmak zorundadır. 0 değeri alamaz. Host ID’leri minimum 1; maksimum 254 olabilir.

### IP (Internet Protocol) Adresi

* Kural 1: 	Bir IP adresinde (Network ve Host ID dahil) 0’dan küçük, 255’ten büyük rakam olamaz!

* Kural 2: 	Host ID’de, 1’den küçük, 254’ten büyük rakam olamaz.

* Kural 3: 	224’ten büyük rakamlı IP’leri de kullanamazsın! 224 ila 255 arasındaki bu aralık, networksel işlemler ve otomatik iletişimler içindir!

* Kural 4: 	127.0.0.1 IP’sini de kullanamazsın! Bu IP, bilgisayarın kendisine tahsistir. Network’teki yerinden bağımsız olarak her bilgisayarın kendisini temsil eder.

### IP (Internet Protocol) Adresi

* IP adreslerinin Network ID ve Host ID’sini belirleyen faktör Subnet Mask (Alt Ağ Maskesi)’dır.

* Subnet Mask’ı belirleyen de IP adresi sınıflarıdır.

* Her IP’nin Subnet Mask’ı ve sınıfı (class) vardır.

### IP (Internet Protocol) Adresi

* Bir ağda 3 tür haberleşme vardır.

    1) 	**Unicast:** Bir cihazdan sadece bir cihaza yapılan iletim.
    
    2) 	**Multicast:** Bir cihazdan belirli bir grup cihaza yapılan iletim.

    3)	**Broadcast:** Bir cihazdan diğer tüm cihazlara yapılan iletim. Network’teki son host IP’si (.255), broadcast için kullanılır.

## AĞ SERVİSLERİ (NETWORK SERVICES)

### Ağ Servisleri

* Ağ ortamında kullanıcılar ve bilgisayarlara hizmet etmesi gereken servisler vardır.

* Örneğin, 

    - **DHCP**, talep eden bilgisayarlara ağa katılması için IP dağıtacaktır. 

    - **DNS**, isim çözmelerine yardımcı olacaktır. 
    
    - **NAT** ise IP çevrimleri yaparak bilgisayarların dış dünyaya açılmasını sağlayacaktır.

### DNS (Domain Name Space):

* Bilgisayarlar birbirileri ile sadece IP’ler ile haberleşirler.

* www.alperentavas.com veya \\SERVER01 gibi adresler bilgisayarlar için bir şey ifade etmez.

* Hedefe ulaşmak isteyen kaynağın, IP adresine ihtiyacı vardır. (LAN’da veya WAN’da.)

* Bu isimlerin IP karşılıkları gerekmektedir. İsim çözümlemesi yapılmalıdır. Bunları DNS sunucuları yaparlar.

* DNS sunucusuna, www.alperentavas.com kimdir, IP’si nedir? denir. O da söyler

### DNS (Domain Name Space):
* Bilgisayarlar (Windows) isim çözümlerken, DNS’e gitmeden önce kendi yöntemleriyle denerler.

    - **Hosts Dosyası:** Host isimlerini çözmek içindir. Bilgisayarın diskinde duran sabit bir dosyadır. C:\WINDOWS\System32\Drivers\Etc klasörü içindedir. Manuel olarak doldurulmalıdır. 

    - **Önbellek:** Öğrenilen IP’lerin, tekrar istenmesi halinde geçici süreliğine tutulduğu bellektir. Bu geçici süreyi belirleyen değer TTL (Time-to-Live)’dır.

    - **DNS Sunucu:** Veritabanında host ve IP isimlerini tutan sunucudur. İstemcilerin (Client’ların) sorgu yapabilmesi için DNS sunucuyu tanıtmaları gerekir. Örneğin 192.168.2.1 (Modem) veya 8.8.8.8 (Google) gibi.

    - **Broadcast:** Bilgisayarların isimlerini çözmek için tüm ağa çağrı yapılmasıdır.

### DNS (Domain Name Space):

* **DNS Resolver (DNS Çözücü):**
DNS sunucularına sorgu atan, client’larda (istemcilerde) çalışan servistir. Internet Browser da (Chrome veya Firefox da) birer resolver’dır.

* **Resource Records (Kaynak Kayıtları):**
Client’lardan gelen sorguları yanıtlamak için kullanılan, DNS veritabanındaki bilgilerdir. Her DNS sunucu resoruce records’a sahiptir.

* **Query (Sorgu):**
Client’ların DNS sunucuya veya DNS sunucunun diğer bir DNS sunucuya gönderdiği isim çözümleme istekleridir. Recursive (Client-Server) ve Iterative (Server-Server) olmak üzere 2 tip sorgu vardır.

### DNS (Domain Name Space):

* **DNS Resolver (DNS Çözücü):**

    - Resolver servisi tarafından kaydedilmiş sorguları görmek için; Komut İstemcisi (Command Prompt/CMD)’ne

        - ipconfig /displaydns

    - Kaydedilmiş sorguları silmek için; Komut İstemcisi (Command Prompt/CMD)’ne
        - ipconfig /flushdns

### DNS (Domain Name Space):

* İnternet’teki DNS’ler hiyerarşik bir isimlendirme metodu kullanırlar. Ağaç şeklinde domain grup’ları ve bu domain grup’larının alt grupları şeklindedir. Bütün domain’ler Root (kök) adı verilen tek bir domain’de birleşirler. Tüm domain’ler Root domain’in üyesidir. Bu yapıya DNS Hiyerarşisi (DNS Hierarchy) denir.

* **FQDN (Fully Qualified Domain Name):**
DNS ağıcında/hiyerarşisinde bir bilgisayarın tam adresini belirten tamamlanmış addır. mail.google.com bir FQDN’dir.

* **Zone (Bölge):**
DNS sunucunun yetkili olduğu bölge, alandır. Bir DNS sunucusu birden fazla bölgeden sorumlu olabilir.

### DHCP (Dynamic Host Configuration Protocol):

* Ağdaki bilgisayarlara IP adresi, Alt Ağ Maskesi (Subnet Mask), Varsayılan Ağ Geçidi (Default Gateway), DNS Server bilgilerini dağıtan servistir.

* IP’lerin benzersiz olması için IP çakışmalarını önler.

* Verilen IP’lerin ömür boyu olmaması için geçici süreliğine kiralar. Varsayılan kira süresi 8 gündür.

* Biten kira süresinin ardından tekrar IP dağıtır.

* Dağıtılan IP aralığının içinden istenmeyen bir aralık dağıtımdan dışlanabilir. Buna Exclusion Range denir.

* Farklı IP istemeyen, sürekli aynı IP’sini kullanması gereken client’lara MAC adresiyle rezervasyon yapar.

* DHCP kullanılmayan ağlarda IP adresi ve diğer bilgiler her client’a manuel girilmek zorundadır.

* Client’lar IP adreslerini otomatik olarak alabilmek için ortamdaki DHCP sunucunu bilmelidirler.

* Bunu, ağa broadcast yayını yaparak öğrenirler. Süreç şöyledir:

    - **DHCP Discover (DHCP Keşfi):** İlk kez IP alacak olan client, broadcast yayını yapar. Bu yayına DHCPDISCOVER adı verilir. Bu yayının içine MAC adresini de ekler.

    - **DHCP Offer (DHCP Teklifi):** Yayını alan DHCP sunucusu ağa DHCPOFFER mesajı yayınlar. Bu mesaj boroadcast’tir; tüm client’lara gider fakat içinde MAC bilgisi olduğu için sadece ilgilisi alır.

    - **DHCP Request (DHCP İsteği):**   Client, DHCP’den gelen teklifi kabul ederse DHCPREQUEST yayını ile cevap verir. Bu mesaj da broadcast’tir.

    - **DHCP Acknowledgement (DHCP Onayı):** DHCP, isteği kabul ettiğini DHCPACK broadcast yayınıyla duyurur ve client, IP adresi edinmiş olur.

### APIPA (Automatic Private IP Addressing):
* DISCOVERY yayınına bir DHCP’den cevap alamayan client, ağ IP’si alamaz.

* Fakat kendine bir IP atar. Buna APIPA (Automatic Private IP Addressing) denir.

* APIPA IP’si 169.254.x.x şeklindedir; subnet’i ise 255.255.0.0’dır.

* APIPA IP’si almış diğer client’lar ile görüşebilir.

### NAT (Network Address Translation):

* Bir network için geçerli 2 tür IP vardır:

    1) Private IP: Lokal network’te (LAN’da) kullanılan IP’lerdir. Lokal network’e aittirler. İç IP’lerdir. 

    2) Public IP: Dış network’te (WAN’da) kullanılan IP’lerdir. İnternet’e aittirler. Dış IP’lerdir.

* NAT, bu ağlar arasında IP çevirme işini yapar. 

* Public (WAN) ve Private (LAN) ağlarının birbiriyle haberleşebilmelerini sağlar.

* Bilgisayarınızın IP’si Private IP’dir. 

* Evinizin IP’si Public IP’dir.

* Modeminizin eve bakan bacağında Private IP; internete bakan bacağında Public IP vardır.

    - Örneğin;
    
        * 192.168.2.1(Private IP) (İç IP)

        * 88.249.51.113   (Public IP) (Dış IP)

### NAT (Network Address Translation):

* Client’ın 192.168.2.10 Private IP’si 3000 portu ile, Server’ın 85.74.114.25 Public IP’sinin 80 portu ile haberleşemez. Çünkü farklı network’teler. Network ID’leri, subnet’leri farklı…

* Araya NAT girerse haberleşebilirler…

* Modem’de, İnternet Hizmet Sağlayıcı (ISP) tarafından atanan bir Public IP vardır.

* NAT, client’ın Private IP’sini, modemin Public IP’si ile değiştirerek hedefe gönderir. Ve böylelikle haberleşebilirler. Bu çevrim işi tersi yönde de gerçekleşir.

