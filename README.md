Bu proje C# dilinde yazılmıştır ve aşağıdaki bileşenleri içerir:

IPerson Interface: Login ve BilgiGoster metodlarını tanımlar.
Kisi Abstract Class: Öğrenciler ve öğretim görevlilerinin ortak özelliklerini içerir.
Ogrenci Class: Öğrencilerin ders kaydı ve bilgilerini tutar.
OgretimGorevlisi Class: Öğretim görevlilerinin dersleri ve bilgilerini tutar.
Ders Class: Ders bilgileri ve öğrenci kayıtlarını içerir.
Sınıflar ve İşlevler

IPerson Interface
IPerson arayüzü, tüm kişi türlerinin (Öğrenci ve Öğretim Görevlisi) uygulaması gereken iki temel metod içerir:

Login(): Kullanıcı girişini simüle eder.
BilgiGoster(): Kullanıcının bilgilerini ekrana yazdırır.
Kisi Abstract Class
Kisi sınıfı, IPerson arayüzünü uygular ve ortak özellikleri içerir:

Ad: Kişinin adı.
Soyad: Kişinin soyadı.
Login(): Kullanıcının girişini ekrana yazar.
BilgiGoster(): Soyut metod olarak tanımlanır ve türetilen sınıflarda özelleştirilir.
Ogrenci Class
Ogrenci sınıfı, öğrencilerin ders kaydını tutar ve BilgiGoster metodunu özelleştirir:

OgrenciNo: Öğrencinin numarası.
Dersler: Öğrencinin kayıtlı olduğu dersler.
DersEkle(Ders ders): Öğrencinin bir derse kaydolmasını sağlar.
OgretimGorevlisi Class
OgretimGorevlisi sınıfı, öğretim görevlilerinin dersleri ve bilgilerini tutar:

SicilNo: Öğretim görevlisinin sicil numarası.
Dersler: Öğretim görevlisinin verdiği dersler.
DersEkle(Ders ders): Öğretim görevlisinin bir dersi eklemesini sağlar.
Ders Class
Ders sınıfı, ders bilgilerini ve dersin öğrenci listesini tutar:

Ad: Dersin adı.
Kredi: Dersin kredi bilgisi.
OgretimGorevlisi: Dersin öğretim görevlisi.
Ogrenciler: Dersin öğrencileri.
KayitOl(Ogrenci ogrenci): Bir öğrenciyi derse kaydeder.
Kullanım

Proje, aşağıdaki adımları takip ederek çalıştırılabilir:

OgretimGorevlisi ve Ders Nesneleri Oluşturma:
İlk olarak bir öğretim görevlisi nesnesi oluşturulur. Bu nesne, dersleri eklemek için kullanılır.
Öğrenciler ve Dersler Arasındaki Bağlantı:
Öğrenciler derslere kaydolur. Öğrenci bir derse kaydolduğunda, ders de öğrenci listesine eklenir.
Bilgilerin Görüntülenmesi:
Hem dersler hem de öğrenciler hakkında detaylı bilgi görüntülenebilir. Her dersin ve öğrencinin bilgileri ekrana yazdırılır.


