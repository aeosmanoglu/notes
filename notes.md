- [1. Bilgisayar Mühendisliğine Giriş](#1-bilgisayar-mühendisliğine-giriş)
  - [1.1. Temel Kavramlar](#11-temel-kavramlar)
  - [1.2. Algoritma ve Akış Şemaları](#12-algoritma-ve-akış-şemaları)
    - [1.2.1. Algoritmada Olması Gereken Özellikler](#121-algoritmada-olması-gereken-özellikler)
    - [1.2.2. Akış Şeması Simgeleri](#122-akış-şeması-simgeleri)
  - [1.3. Programlama Dilleri](#13-programlama-dilleri)
    - [1.3.1. Yazılım Geliştirme Süreci](#131-yazılım-geliştirme-süreci)
    - [1.3.2. Programlama Dilinin Önemi](#132-programlama-dilinin-önemi)
    - [1.3.3. Nesneye Yönelik Programlama](#133-nesneye-yönelik-programlama)
    - [1.3.4. Programlama Ortamı](#134-programlama-ortamı)
  - [1.4. İşletim Sistemleri](#14-i̇şletim-sistemleri)
    - [1.4.1. Bilgisayar Sistemi Bileşenleri](#141-bilgisayar-sistemi-bileşenleri)
    - [1.4.2. İşletim Sistemlerinin Temel İşlevleri](#142-i̇şletim-sistemlerinin-temel-i̇şlevleri)
    - [1.4.3. Sistem Performansı](#143-sistem-performansı)
    - [1.4.4. Çekirdek Sistem](#144-çekirdek-sistem)
    - [1.4.5. Proses Yönetimi](#145-proses-yönetimi)
    - [1.4.6. Bellek Yönetimi](#146-bellek-yönetimi)
- [2. Bilgisayar Mimarisi ve Tasarım](#2-bilgisayar-mimarisi-ve-tasarım)
- [3. Bilgisayar Ağları](#3-bilgisayar-ağları)
- [4. Veri Yapıları ve Algoritmalar](#4-veri-yapıları-ve-algoritmalar)
- [5. Java ile Programlama](#5-java-ile-programlama)
- [6. İşletim Sistemleri](#6-i̇şletim-sistemleri)
  - [6.1. Bilgisayarlar ve İşletim Sistemleri](#61-bilgisayarlar-ve-i̇şletim-sistemleri)
  - [6.2. Bilgisayar Mimarileri](#62-bilgisayar-mimarileri)
    - [6.2.1. CISC (complex instruction set computer) Mimarisi](#621-cisc-complex-instruction-set-computer-mimarisi)
    - [6.2.2. RISC (reduced instruction sasetid computer) Mimarisi](#622-risc-reduced-instruction-sasetid-computer-mimarisi)
    - [6.2.3. İşletim Sistemleri Ağ Özellikleri](#623-i̇şletim-sistemleri-ağ-özellikleri)
- [7. Veri Tabanı Yönetim Sistemleri](#7-veri-tabanı-yönetim-sistemleri)
- [8. Yazılım Mühendisliği](#8-yazılım-mühendisliği)
- [9. Web Programlama](#9-web-programlama)
- [10. Yazılım Proje Yönetimi](#10-yazılım-proje-yönetimi)

# 1. Bilgisayar Mühendisliğine Giriş

## 1.1. Temel Kavramlar

> **Birleşik mantık devreleri** VE, VEYA gibi kapılardan oluşur ve devrenin çıktısı sadece o anki girdilere bağlıdır. **Sıralı/Ardışıl mantık devreleri (flip-flop)** hem o andaki girdilere hem de bir önceki çıktıya bağlıdır. Bu devreler saat darbeleri ile çalışır.

> Assembly diliyle yazılmış programların çalışması için makina koduna dönüştürülmesi gerekir. Her işlemci ailesinin kendine has makina kodu ve assembly dili vardır.

## 1.2. Algoritma ve Akış Şemaları

### 1.2.1. Algoritmada Olması Gereken Özellikler

1. Etkin ve Genel olma
1. Sonlu olma
1. Yanılmazlık
1. Giriş/Çıkış tanımlı olma
1. Başarım (Bellek gereksinimi ve çalışma süresi arasındaki denge)

### 1.2.2. Akış Şeması Simgeleri

:::mermaid
flowchart TD
id1([Başla])
id2([Dur])
id3[/Klavye/]
İşlem
id4[[Fonksiyon]]
id5{Koşul}
id6{{Döngü}}
id7[(Veri Tabanı)]
:::

## 1.3. Programlama Dilleri

### 1.3.1. Yazılım Geliştirme Süreci

1. Gereksinim analizi
1. Yazılım Tasarımı
1. Kodlama
1. Sertifikasyon
1. Bakım

### 1.3.2. Programlama Dilinin Önemi

1. Güvenilir olmalı
   1. Yazılabilirlik
   1. Okunabilirlik
   1. Sıra dışı durumları karşılayabilme
1. Bakıma elverişli olmalı
1. Verimli çalışmalı

### 1.3.3. Nesneye Yönelik Programlama

1. **Veri soyutlama:** Yeni veri türlerini modelleyen sınıflar yaratması
1. **Kalıtım:** Sınıfları genişleterek ve özelleştirerek yeni sınıflar türetilmesi
1. **Çok biçimlilik:** Aynı isimdeki işlemlerin değişik nesne sınıfları için farklı algılanması

### 1.3.4. Programlama Ortamı

1. Editör
1. Derleyici (Compiler)
1. Kütüphane (Librarian): Nesne dosyaları
1. Bağlayıcı (Linker): Tüm nesne dosyalarını birleştirerek tek bir yürütülebilir dosya haline getirir
1. Yükleyici (Loader): Yürütülebilir dosyayı diskten belleğe kopyalar
1. Hata ayıklayıcı
1. Yorumlayıcı (Interpreter): Bir programın kaynak kodunu doğrudan satır satır yürüten program

:::mermaid
flowchart LR

Kaynak-->s1

subgraph s1 [Ön Uç]
a[sözdizimi cümleleme]-->b[anlam çözümleme]
end
s1-->1[Arka Kod]

subgraph s2 [Arka Uç]
x[makineden bağımsız eniyileme]-->y[kod üretimi]-->z[makineye bağımlı eniyileme]
end
s2-->2[Makine Kodu]
:::

## 1.4. İşletim Sistemleri

### 1.4.1. Bilgisayar Sistemi Bileşenleri

1. Donanım
2. İşletim sistemi
3. Sistem ve uygulama programları
4. Kullanıcılar

### 1.4.2. İşletim Sistemlerinin Temel İşlevleri

1. Yazılım donanım bütünlüğünün sağlanması
2. Kaynakların yönetimi
   1. Görev (task) > İş (job)
3. Kullanıcı ile sistem arasındaki ilişki, uyum ve düzen
   1. Adanmış işlem (dedicated)
   2. Toplu işlem (batch)
   3. Etkileşimli işlem (interactive, time sharing)

### 1.4.3. Sistem Performansı

1. **Verimlilik:** Sistem kaynaklarının düşük kullanımı
2. **Güvenilirlik:** Donanım ve yazılım yüzünden doğacak sorunları sezebilmeli ve önlemeli
3. **Koruyuculuk:** Bir kullanıcının yaptığı hatadan diğer kullanıcı etkilenmemeli
4. **Sezdiricilik**
5. **Elverişlilik:** Kullanıcı sistemin kaynaklarını kendi isteğine göre değil sistemin izin verdiği ölçüde kullanmalı

### 1.4.4. Çekirdek Sistem

1. İşlemciye prosesleri atamak
2. Kesmeleri yönetmek
3. Prosesler arasında iletişimi sağlamak

### 1.4.5. Proses Yönetimi

> **Proses:** kendi veri şablonu olan ve kendi başına bütünlüğü olan kod parçası

1. Çalışıyor (running)
2. Askıda (blocked)
3. Hazır (ready)

> **Zaman Çizelgeleyici (schedular):** İşlemciye atanacak olan prosesi ve prosesin hangi koşullar altında işlemciyi kullanacağını belirler.

1. Proses kuyruğundan yürütülecek prosesi seçer
2. Prosesin kullanım zaman dilimini ayarlar

> **Deadlack:** proseslerin hiç bir zaman ele geçiremeyecekleri bir birim veya kaynağa ihtiyaç duymaları sebebiyle sürekli askıda kalması

> **Semafor:** Bir çeşit değişken. Signal ve Wait'tir.

### 1.4.6. Bellek Yönetimi

| Bellek                           | Statik/Dinamik | Gerçek/Sanal |
| -------------------------------- | -------------- | ------------ |
| Tekli kesintisiz                 | S              | G            |
| Bölümlenmiş                      | S              | G            |
| Yer değiştirilebilir bölümlenmiş | D              | G            |
| Sayfalı                          | D              | G            |
| İsteğe bağlı sayfalı             | D              | S            |
| Dilimli                          | D              | S            |
| Dilimli ve isteğe bağlı sayfalı  | D              | S            |

# 2. Bilgisayar Mimarisi ve Tasarım

# 3. Bilgisayar Ağları

# 4. Veri Yapıları ve Algoritmalar

# 5. Java ile Programlama

# 6. İşletim Sistemleri

## 6.1. Bilgisayarlar ve İşletim Sistemleri

:::mermaid
flowchart LR
2(Uygulama Programları)
1(Kullanıcı)
3(Kabuk)
4(Sistem Çağrıları Arayüzü)
5(Çekirdek)
6(Donanım)
subgraph Bilgisayar Sistemi
1<-->2
1<-->3
2<-->3
subgraph İşletim Sistemi
3<--Kullanıcı Kipi-->4
4<--Çekirdek Kipi-->5
end
5<-->6
end
:::

## 6.2. Bilgisayar Mimarileri

|                       | Harvard Mimarisi                                              | von Neumann Mimarisi                                                             |
| --------------------- | ------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Düzenleme             | ROM komutlar, RAM veri için. Belleğe erişim yolları bağımsız. | ROM bilgisayarın açılışı, RAM veri ve kodlar için. Belleğe erişim yolları ortak. |
| Donanım Gereksinimi   | Karmaşık                                                      | Basit                                                                            |
| Alan Gereksinimi      | Çok                                                           | Az                                                                               |
| Komut Çalıştırma Hızı | Yüksek                                                        | Düşük                                                                            |
| Bellek Alan Kullanımı | Çok                                                           | Az ve efektif                                                                    |
| Kontrol Karmaşıklığı  | Yüksek                                                        | Az                                                                               |

### 6.2.1. CISC (complex instruction set computer) Mimarisi

CISC mimarisi yüksek seviyeli programlama dillerindeki ifadelerin makine dilinde benzer şekilde doğrudan ifade edilmesine imkan sağlayacak şekilde tasarlanmıştır. Bunun gereği olarak CISC mimarisinde komut yapısı operantlardan en az bir tanesinin birlikte olmasını öngörür ve komutlar birden fazla alt operasyondan oluşurlar.

### 6.2.2. RISC (reduced instruction sasetid computer) Mimarisi

CISC mimarisi kullanıcı odaklı iken RISC mimarisi donanım odaklı bir tasarıma sahiptir. RISC mimarisinde alt operasyonların böl ve yönet mantığına göre bellekten okuma, aritmetik lojik işlem yapma ve belleğe yazma olmak üzere birbirinden bağımsız üç ayrı komik şekilde ifade edilmesi ile ortadan kaldırmıştır. Bu yaklaşımın sonucu RISC mimarisindeki bütün komutların uzunluğu birbirine eşittir ve aritmetik lojik i̇şlemler sadece saklıcılar içinde gerçekleştirilir.

```
/* CISC */
MULT Addr1, Addr2

/* RISC */
LOAD A, Addr1
LOAD B, Addr2
PROD A, B
STORE Addr1, A

```

| CISC                                               | RISC                                              |
| -------------------------------------------------- | ------------------------------------------------- |
| donanıma yük biner                                 | yazılıma yük biner                                |
| çok saat döngüsü ile çalışan karmaşık komutlar     | tek saat döngüsünde tamamlanabilen basit komutlar |
| az birleştirici kodu                               | çok birleştirici kodu                             |
| transistörler karmaşık kod tasarım için kullanılır | transistörler saplayıcılar için kullanılır        |

### 6.2.3. İşletim Sistemleri Ağ Özellikleri

**Linux:** Kullanıcı uygulamaları tüm isteklerini soket arabirimi üzerinden gerçekleştirir. Linux ağ katmanı BSD soket katmanı alt yapısı üzerine inşa edilmiştir. Herhangi bir ağ verisi bu katmana bir uygulamanın soketinden veya bir ağ aygıtı sürücüsünden geldiğinde verilerin hangi ağ protokolünü içerdiklerini belirten bir tamamlayıcıyla etiketlenmiş olması beklenir.

**Windows:** Ağ arttırım protokollerini sürücüler üzerinden uygulamaktadır.

1.  Sunucu ileti blogu (SMB) protokolü: Sistem üzerinden giriş çıkış isteklerinin gönderilmesi, oturumunda denetimi, sunucudan kaynana yönlendirme bağlantısını başlatan ve sonlandıran, yeniden yönlendirme süreçlerini yöneten, dosyalara erişim kontrollerini yapan, ağ üzerindeki yazılara veri gönderim süreçleri yöneten protokol. Yeni adıı Ortak İnternet Dosya Sistemi (CIFS)
2.  İletim Kontrol Protokolü: Basit ağ Yönetim Protokolü (SNMP), dinamik ana bilgisayar yapılandırma protokolü (DHCP) ve Windows İnternet Ad (WINS) gibi hizmetleri içerir.
3.  Noktadan noktaya tünel protokolü (PPTP)
4.  HTTP
5.  Uzaktan Yordan Çağrıları (RPC)/(VPN)
6.  Bileşen nesne modeli (COM)/(DCOM)

# 7. Veri Tabanı Yönetim Sistemleri

# 8. Yazılım Mühendisliği

# 9. Web Programlama

# 10. Yazılım Proje Yönetimi
