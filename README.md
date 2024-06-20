# SlimBuddy Gereksinim Analizi Belgesi

# 1.1 Sistemin Amacı

SlimBuddy programı kullanıcıların günlük kalori takiplerini yapmalarına ve öğünlerini planlayıp, 

özelleştirmelerine, haftalık ve günlük bazda karşılaştırma yapmalarına olanak tanıyacak şekilde

tasarlanmıştır.

# 1.2 Sistemin Kapsamı

Program, kullanıcıların günlük öğünlerini izlemelerine yardımcı olacak bir WinForm uygulaması olarak 

tasarlanmıştır. Program aşağıdaki temel özelliklere sahiptir;

i. Yeni kullanıcılar oluşturulabilir ve mevcut kullanıcılar oturum açabilir.

ii. Kullanıcılar, günlük öğünlerinin girişini yapabilir, güncelleyebilir veya silebilir.

iii. Program, kullanıcının cinsiyeti, kilosu, boyu, yaşının yanı sıra aktivite seviyesi gibi bilgileri 

kullanarak günlük alması gereken kilo miktarını hesaplayacaktır.

iv. Kullanıcılar, programda bulunmayan bir yiyeceği sisteme ekleyebileceklerdir.

# 1.3 Projenin hedefleri ve başarı kriterleri

i. Kullanıcıların kolayca yeni hesaplar oluşturabilmesi ve oturum açabilmesi.

ii. Kullanıcıların günlük öğünlerini eklemesi, güncellemesi ve silebilmesi.

iii. Programın, kullanıcının aktivite durumuna göre günlük kalori ihtiyacının doğru bir şekilde 

hesaplanması.

iv. Kullanıcıların, programda bulunmayan yiyecekleri kolayca sisteme ekleyebilmesi.

v. Arayüzün kullanıcı dostu olması ve kullanıcıların işlemleri kolayca gerçekleştirebilmesi.

vi. Programın güvenilir olması , kullanıcıların veri kaybı veya hatalarla karşılaşmaması.

Bu hedefler ve başarı kriterleri, projenin başarılı bir şekilde tasarlanması için belirlenen ölçütleri 

ve hedefleri temsil eder. Bu hedefler projenin gereksinimlerini ve kullanıcı ihtiyaçlarını karşılayacak 

şekilde belirlenmiştir.

# 1.4 Tanımlar , kısaltmalar 

i. GAB: Gereksinim Analizi Belgesi

ii. WinForms: Windows Forms

iii. Vb.: Ve benzeri

iv. GUI: Grafiksel Kullanıcı Arayüzü

v. Kcal: Kilo Kalori

1.5 Kaynaklar

i. Visual Studio belgeleri

ii. .NET Framework dökümantasyonu

iii. Benzer uygulamaların analiz belgeleri

iv. MS SQL Server dökümantasyonu

# Kullanılan Teknolojiler

i. Geliştirme Ortamı: Ms Visual Studio 2022

ii. Kod Altyapısı: C#, .NET CORE 8.0

iii. Mimari Tasarım: N-Tier Katmanlı Mimari

iv. Veri Tabanı: Ms SQL Server

v. Veri Erişim Teknolojisi: Entity Framework CORE (CodeFirst)

vi. Arayüz Tasarımı: Windows Forms Application

vii. Versiyon Kontrol Sistemi: Git

# 1.6 Genel Bakış

Bu belge, SlimBuddy programının gereksinimlerini belirlemek ve analiz etmek için oluşturulmuştur. 

Program, kullanıcıların günlük kalori alımlarını izlemelerine, öğünlerini planlamalarına ve 

düzenlemelerine olanak tanıyacak şekilde tasarlanacaktır.

Proje, kullanıcıların sağlıklı bir yaşam tarzını sürdürebilmeleri için teşvik sağlar ve günlük beslenme 

alışkanlıklarını izleyebilmeleri için kullanışlı bir araç sunmayı hedeflemektedir. Program, kullanıcı 

dostu bir arayüzle tasarlanacak ve temel işlevselliği kolayca erişilebilir hale getirecektir.

Bu belge proje ekibi ve ilgili taraf arasında bir anlayış ve birlik sağlamak için kullanılacaktır.

# 2.Önerilen Sistem

# 2.1 Genel Bakış

Sistem kullanıcıların günlük kalori alımlarını izlemelerini sağlamak, öğünlerini planlamalarına ve 

düzenlemelerine olanak tanımak amacıyla tasarlanmıştır. Aşağıda sistemin ana işlevselliği 

özetlenmiştir;

Kullanıcı Hesapları: Yeni kullanıcı oluşturulabilir ve mevcut kullanıcılar oturum açabilir.

Admin Hesabı: Admin kullanıcıları Active ve Passive’e çekip programa girişlerine izin verir ya da 

engeller.

Öğün Yönetimi: Kullanıcılar, günlük öğünlerini ekleyebilir ve silebilir.

Kalori Hesaplama: Program, kullanıcının cinsiyeti, kilosu, boyu, yaşı, günlük aktivite seviyesi gibi 

bilgileri kullanarak günlük alması gereken kcal miktarını hesaplar. Bunun yanı sıra kullanıcının 

öğünlerinin toplam kcal hesabını yapar.

Yiyecek Ekleme: Kullanıcılar, programda bulunmayan bir yiyeceği sisteme yiyeceğin fotoğrafı ile 

ekleyebilirler.

Analiz: Kullanıcı öğünlerinin, günlük ve haftalık bazda kendisiyle ve diğer kullanıcılarla kıyaslamasını 

yapabilir.

Gün Sonu Raporu : İlgili gün kullanıcı yediği öğünlerin kcal olarak toplamını görebilir.

# 2.2 Fonksiyonel Gereksinimler (“listeler”)

A) Kullanıcı İşlevselliği

i. Yeni kullanıcı oluşturma

ii. Oturum açma

iii. Kullanıcı bilgilerini güncelleme

B) Öğün İşlevselliği

i. Öğün ekleme

ii. Öğün güncelleme

iii. Öğün silme

C) Yiyecek İşlevselliği

i. Tanımlı yiyeceklere ulaşma

ii. Yeni yiyecek ekleme

iii. Yiyecek güncelleme

D) Kalori Hesaplama İşlevselliği

i. Günlük kcal ihtiyacı hesaplama

ii. Öğünlerdeki yiyeceklerin toplam kcal hesabını yapma

E) Raporlama İşlevselliği

i. Öğün bazlı kcal raporu

ii. Günlük ve haftalık olarak karşılaştırma raporu

2.3 Fonksiyonel Olmayan Gereksinimler

2.3.1 Kullanılabilirlik

GUI, kullanıcıların etkileşimi zorlanmadan yapabileceği şekilde tasarlanacaktır. Program içerisinde var 

olan özelliklere kolayca gezinerek erişebilinecektir.

2.3.2 Güvenilirlik 

Kullanıcının veri bütünlüğünü sağlamak için uygun önlemler alınacaktır. Uygulama kullanıcıya anlaşılır 

hata mesajları sağlayarak hata durumlarını ele alacaktır.

2.3.3 Performans

Uygulama, kullanıcıların isteklerine hızlı bir şekilde yanıt verecek ve gecikmeler minimumda 

tutulmaya çalışılacaktır.

2.3.4 Desteklenebilirlik

Kod, kolayca anlaşılabilinmesi ve sonradan eklenecek farklı işlevselliklerin uygulanabilmesi için açık 

bir şekilde yazılacaktır. Bu kodun kolay yönetilebilinmesini de sağlayacaktır.

2.3.5 Uygulama

Uygulama farklı Windows platformlarında sorunsuz çalışacaktır.

2.3.6 Arayüz

Arayüz kullanıcıların rahatlıkla kullanabileceği ve anlaşılır olacaktır. Arayüz görsel açıdan kullanıcıları 

memnun edecek şekilde tasarlanacaktır.

2.4 Sistem Modelleri

2.4.1 Senaryolar

Aşağıdaki adımlar kullanıcının uygulamayı işlevsel bir şekilde kullanabilmesi için açıklanmıştır.

i. Uygulama başlatıldığında kullanıcının karşısına Login ekranı gelir.

ii. Kullanıcı Create Account seçeneğinde tıklar ve istenilen bilgileri girerek yeni hesap oluşturur.

iii. Create Account ekranını kapattığında Login ekranı açılır ve hesap bilgilerini girerek 

uygulamaya giriş yapar.

iv. Giriş yapıldığında Meal ekranı açılır. Bu ekranda kullanıcı o gün içerisindeki öğünlerinde yediği 

yemekleri sisteme ekleyebilir.

v. Food ekranına geçtiğinde programda olmayan yiyecekleri ekleyebilir ve daha önce eklediği 

yemekleri görebilir ve isterse güncelleyebilir.

vi. Daily Calorie ekranında o günkü aktivite seviyesine göre alması gereken kalori belirlenir.O gün 

yediği öğünlerin toplam kalorisini görebilir.

vii. Analysis ekranında kullanıcı öğünlerinin, günlük ve haftalık bazda kendisiyle ve diğer 

kullanıcılarla kıyaslamasını yapabilir.

viii. Summary ekranında o gün yediği öğünleri görebilir ve dilerse silebilir.

ix. Account ekranına geçtiğinde ise hesap bilgilerini görebilir ve dilerse güncelleyebilir.

x. Log Out’a bastığında ise programdan çıkış sağlanmış olur. 

2.4.2 Kullanım örneği modeli

2.4.3 Analiz nesnesi modeli

2.4.4 Dinamik model

2.4.5 Kullanıcı arabirimi

Login Screen: Programın açılış ekranıdır. Bu ekrandan hesabı varsa uygulamaya giriş sağlar. Eğer 

hesabı yoksa Create Account ekranına buradan erişir ve bir hesap oluşturur.

Create Account: Bu ekran hesabı olmayan kullanıcının hesap oluşturmasını sağlar.

Admin Panel: Admin hesabın kullanıcının sisteme erişimini izin verdiği ekrandır.

Home Screen: Bu ekranda kullanıcı gün içerisinde yediği öğünlerin girişini yapabilir ve kalorilerini 

görebilir.

Food Screen: Bu ekranda kullanıcı programda olmayan yemekleri ekleyebilir , eklediği yemekleri 

güncelleyebilir ve silebilir.

Daily Calorie Screen: Kullanıcının günlük aktivite seviyesine göre kalori ihtiyacını hesaplayıp gösteren 

ekrandır. Bu ekranda kullanıcı ilgili gün içerisindeki öğünlerinin toplam kalorisini görebilir.

Analysis Screen: Bu ekran kullanıcı öğünlerinin, günlük ve haftalık bazda kendisiyle ve diğer 

kullanıcılarla kıyaslamasını yapabilmesini sağlar.

Summary Screen: Bu ekran kullanıcının o gün yediği öğünleri görebilmesini ve dilerse silebilmesini 


sağlar.

Account Screen: Kullanıcının e-mail adresini,yaşını,boyunu kilosunu gösteren ve bu bilgilerden 

güncellemek istediklerini güncellemesini sağlayan ekrandır.


![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Create%20Account%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Giris%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Admin%20Login%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Account%20Information%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Admin%20Panel%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Food%20Ekleme%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Gunluk%20Kalori%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Gunluk%20Ogun%20Ozeti%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Ogun%20Ekleme%20Ekrani.png)

![](https://github.com/MahmutTaylan/SlimBuddyWinForm/blob/main/Analiz%20Ekrani.png)
