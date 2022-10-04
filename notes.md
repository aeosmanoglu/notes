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
    - [1.4.1. İşletim Sistemlerinin Temel İşlevleri](#141-i̇şletim-sistemlerinin-temel-i̇şlevleri)
    - [1.4.2. Sistem Performansı](#142-sistem-performansı)
    - [1.4.3. Çekirdek Sistem](#143-çekirdek-sistem)
    - [1.4.4. Proses Yönetimi](#144-proses-yönetimi)
    - [1.4.5. Bellek Yönetimi](#145-bellek-yönetimi)
- [2. Bilgisayar Mimarisi ve Tasarım](#2-bilgisayar-mimarisi-ve-tasarım)
- [3. Bilgisayar Ağları](#3-bilgisayar-ağları)
- [4. Veri Yapıları ve Algoritmalar](#4-veri-yapıları-ve-algoritmalar)
- [5. Java ile Programlama](#5-java-ile-programlama)
- [6. İşletim Sistemleri](#6-i̇şletim-sistemleri)
- [7. Veri Tabanı Yönetim Sistemleri](#7-veri-tabanı-yönetim-sistemleri)
- [8. Yazılım Mühendisliği](#8-yazılım-mühendisliği)
- [9. Web Programlama](#9-web-programlama)
- [10. Yazılım Proje Yönetimi](#10-yazılım-proje-yönetimi)

# 1. Bilgisayar Mühendisliğine Giriş

## 1.1. Temel Kavramlar

**Birleşik mantık devreleri** VE, VEYA gibi kapılardan oluşur ve devrenin çıktısı sadece o anki girdilere bağlıdır. **Sıralı/Ardışıl mantık devreleri (flip-flop)** hem o andaki girdilere hem de bir önceki çıktıya bağlıdır. Bu devreler saat darbeleri ile çalışır.

Assembly diliyle yazılmış programların çalışması için makina koduna dönüştürülmesi gerekir. Her işlemci ailesinin kendine has makina kodu ve assembly dili vardır.

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

### 1.4.1. İşletim Sistemlerinin Temel İşlevleri

1. Yazılım donanım bütünlüğünün sağlanması
2. Kaynakların yönetimi
   1. Görev (task) > İş (job)
3. Kullanıcı ile sistem arasındaki ilişki, uyum ve düzen
   1. Adanmış işlem (dedicated)
   2. Toplu işlem (batch)
   3. Etkileşimli işlem (interactive, time sharing)

### 1.4.2. Sistem Performansı

1. **Verimlilik:** Sistem kaynaklarının düşük kullanımı
2. **Güvenilirlik:** Donanım ve yazılım yüzünden doğacak sorunları sezebilmeli ve önlemeli
3. **Koruyuculuk:** Bir kullanıcının yaptığı hatadan diğer kullanıcı etkilenmemeli
4. **Sezdiricilik**
5. **Elverişlilik:** Kullanıcı sistemin kaynaklarını kendi isteğine göre değil sistemin izin verdiği ölçüde kullanmalı

### 1.4.3. Çekirdek Sistem

1. İşlemciye prosesleri atamak
2. Kesmeleri yönetmek
3. Prosesler arasında iletişimi sağlamak

### 1.4.4. Proses Yönetimi

> **Proses:** kendi veri şablonu olan ve kendi başına bütünlüğü olan kod parçası

1. Çalışıyor (running)
2. Askıda (blocked)
3. Hazır (ready)

> **Zaman Çizelgeleyici (schedular):** İşlemciye atanacak olan prosesi ve prosesin hangi koşullar altında işlemciyi kullanacağını belirler.

1. Proses kuyruğundan yürütülecek prosesi seçer
2. Prosesin kullanım zaman dilimini ayarlar

> **Deadlack:** proseslerin hiç bir zaman ele geçiremeyecekleri bir birim veya kaynağa ihtiyaç duymaları sebebiyle sürekli askıda kalması

> **Semafor:** Bir çeşit değişken. Signal ve Wait'tir.

### 1.4.5. Bellek Yönetimi

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

# 7. Veri Tabanı Yönetim Sistemleri

# 8. Yazılım Mühendisliği

# 9. Web Programlama

# 10. Yazılım Proje Yönetimi
