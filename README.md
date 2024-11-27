# Öğrenci ve Ders Yönetim Sistemi
Bu proje, öğrenci, öğretim görevlisi ve ders yönetimini simüle eden bir konsol uygulamasıdır. Kullanıcılar öğrenci ve öğretim görevlisi ekleyebilir, ders tanımlayabilir ve derslere öğrenci kaydedebilir. Ayrıca, öğrenci ve öğretim görevlisi bilgilerini görüntüleyebilirler.

# İçindekiler
*Özellikler
*Kullanıcı Arayüzü
*Sınıflar ve İşlevler
*Lisans
*Özellikler

Öğrenci Tanımlama: Öğrenci adı, soyadı ve ID'si ile öğrenci tanımlama.
Öğretim Görevlisi Tanımlama: Öğretim görevlisi adı, soyadı ve ID'si ile öğretim görevlisi tanımlama.
Ders Tanımlama: Ders adı, kredi bilgisi ve öğretim görevlisi ataması ile ders tanımlama.
Dersin Detayları: Tanımlanan derslerin detaylarını gösterme.
Öğrenci Kaydı: Öğrencinin bir derse kaydolmasını sağlama.
Kayıtlı Öğrencileri Görüntüleme: Dersin hangi öğrenciler tarafından alındığını gösterme.

# Kullanıcı Arayüzü
Proje bir konsol uygulamasıdır ve kullanıcıya çeşitli seçenekler sunar. Uygulama çalıştığında kullanıcı aşağıdaki menüyü görür:

Öğrenci ve Ders Yönetim Sistemi
1. Öğrenci Tanımla
2. Öğretim Görevlisi Tanımla
3. Ders Tanımla
4. Dersin Detaylarını Göster
5. Öğrenci Kaydı Yap
6. Çıkış
Bir seçenek girin:




Öğrenci ve Ders Yönetim Sistemi
Bu proje, öğrenci, öğretim görevlisi ve ders yönetimini simüle eden bir konsol uygulamasıdır. Kullanıcılar öğrenci ve öğretim görevlisi ekleyebilir, ders tanımlayabilir ve derslere öğrenci kaydedebilir. Ayrıca, öğrenci ve öğretim görevlisi bilgilerini görüntüleyebilirler.

İçindekiler
Özellikler
Nasıl Çalıştırılır?
Kullanıcı Arayüzü
Sınıflar ve İşlevler
Lisans
Özellikler
Öğrenci Tanımlama: Öğrenci adı, soyadı ve ID'si ile öğrenci tanımlama.
Öğretim Görevlisi Tanımlama: Öğretim görevlisi adı, soyadı ve ID'si ile öğretim görevlisi tanımlama.
Ders Tanımlama: Ders adı, kredi bilgisi ve öğretim görevlisi ataması ile ders tanımlama.
Dersin Detayları: Tanımlanan derslerin detaylarını gösterme.
Öğrenci Kaydı: Öğrencinin bir derse kaydolmasını sağlama.
Kayıtlı Öğrencileri Görüntüleme: Dersin hangi öğrenciler tarafından alındığını gösterme.
Nasıl Çalıştırılır?
Bu uygulama C# dilinde yazılmıştır ve Visual Studio veya başka bir C# IDE'sinde çalıştırılabilir. Aşağıdaki adımları izleyerek projeyi çalıştırabilirsiniz:



Kullanıcı Arayüzü
Proje bir konsol uygulamasıdır ve kullanıcıya çeşitli seçenekler sunar. Uygulama çalıştığında kullanıcı aşağıdaki menüyü görür:

Öğrenci ve Ders Yönetim Sistemi
1. Öğrenci Tanımla
2. Öğretim Görevlisi Tanımla
3. Ders Tanımla
4. Dersin Detaylarını Göster
5. Öğrenci Kaydı Yap
6. Çıkış
Bir seçenek girin:

Kullanıcı, bu menüdeki seçeneklerden birini girerek işlem yapabilir. Seçeneklerin anlamı şu şekildedir:

1 Öğrenci Tanımla: Yeni bir öğrenci ekler.
2 Öğretim Görevlisi Tanımla: Yeni bir öğretim görevlisi ekler.
3 Ders Tanımla: Yeni bir ders tanımlar.
4 Dersin Detaylarını Göster: Tanımlanan dersin detaylarını gösterir.
5 Öğrenci Kaydı Yap: Öğrenciyi bir derse kaydeder.
6 Çıkış: Uygulamadan çıkılır.

# Sınıflar ve İşlevler
Person Sınıfı
Person sınıfı, tüm kişileri (öğrenci ve öğretim görevlisi) temsil eden temel bir sınıftır. Bu sınıf aşağıdaki özelliklere sahiptir:

Name: Kişinin adı.
Surname: Kişinin soyadı.
Id: Kişinin ID numarası.
Ve şu metodları içerir:

BilgiGoster(): Kişinin adı, soyadı ve ID'sini gösterir.
ILogin Arayüzü
ILogin arayüzü, Login() metodunu içerir. Hem Ogrenci hem de OgretimGorevlisi sınıfları bu arayüzü implement eder.

Ogrenci Sınıfı
Ogrenci sınıfı, Person sınıfından türetilmiştir ve ILogin arayüzünü implement eder. Bu sınıf aşağıdaki özelliklere sahiptir:

EnrolledCourses: Öğrencinin kayıtlı olduğu derslerin listesi.
Ve şu metodları içerir:

Login(): Öğrencinin giriş yapmasını simüle eder.
BilgiGoster(): Öğrencinin bilgilerini ve kayıtlı olduğu dersleri gösterir.
RegisterCourse(): Öğrencinin bir derse kaydını yapar.
OgretimGorevlisi Sınıfı
OgretimGorevlisi sınıfı, Person sınıfından türetilmiştir ve ILogin arayüzünü implement eder. Bu sınıf aşağıdaki özelliklere sahiptir:

Courses: Öğretim görevlisinin verdiği derslerin listesi.
Ve şu metodları içerir:

Login(): Öğretim görevlisinin giriş yapmasını simüle eder.
BilgiGoster(): Öğretim görevlisinin bilgilerini ve verdiği dersleri gösterir.
AddCourse(): Öğretim görevlisinin bir ders eklemesini sağlar.
Course Sınıfı
Course sınıfı, dersleri temsil eder ve aşağıdaki özelliklere sahiptir:

Name: Ders adı.
Credits: Dersin kredisi.
Instructor: Dersi veren öğretim görevlisi.
EnrolledStudents: Derse kayıtlı öğrenciler.
Ve şu metodları içerir:

EnrollStudent(): Öğrencinin derse kaydını yapar.
ShowCourseDetails(): Dersin detaylarını (ad, kredi, öğretim görevlisi, öğrenciler) gösterir.

# Lisans
https://github.com/mehmetkbts


