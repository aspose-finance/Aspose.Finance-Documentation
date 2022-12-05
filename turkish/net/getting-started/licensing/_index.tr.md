---
title: lisanslama
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /tr/net/licensing/
description: C# Finance Kütüphane API müşterilerini Klasik lisans ve Sayaçlı Lisans almaya davet ediyor. Ürünü daha iyi keşfetmek için sınırlı bir lisans kullanmanın yanı sıra.
---
## **Değerlendir Aspose.Finance**
Aspose.Finance for .NET ürününü değerlendirme amaçlı kolayca indirebilirsiniz. Lütfen şuraya bakın:[Aspose.Finance for .NET indirme sayfası](https://www.nuget.org/packages/Aspose.Finance/)en son sürümü öğrenmek için. Değerlendirme sürümü, bileşenin lisanslı sürümüyle kesinlikle aynı yetenekleri sağlar. Ayrıca, lisansı uygulamak için birkaç satır kod eklediğinizde, değerlendirme sürümü kolayca lisanslanır.

### **Değerlendirme Sürümü Sınırlamaları**
Değerlendirme sürümü, aşağıdakiler dışında tüm özellikleri sağlar:

- **Açılan Dosya Sayısı** (Aspose.Finance) Programınızı çalıştırırken Aspose.Finance kütüphanesini kullanarak sadece 50 dosya açabilirsiniz. Uygulamanız bu sayıyı aşarsa bir istisna atılır.
- **Kayıtlı Dosya Sayısı** (Aspose.Finance) Programınızı çalıştırırken Aspose.Finance kütüphanesini kullanarak sadece 50 dosya açabilirsiniz. Uygulamanız bu sayıyı aşarsa bir istisna atılır.

{{% alert color="primary" %}} 

 Aspose.Finance'i değerlendirme kısıtlamaları olmadan denemek istiyorsanız, 30 günlük geçici bir lisans talep edin. Bakınız[Geçici Lisans nasıl alınır?](https://purchase.aspose.com/temporary-license) daha fazla bilgi için.

{{% /alert %}} 
## **Bir Lisansın Uygulanması**
 kendinle mutlu olduktan sonra[değerlendirme](https://downloads.aspose.com/finance/net) Aspose.Finance for .NET, Aspose web sitesinden bir lisans satın alın:[Satın Alma Portalı](https://purchase.aspose.com/buy) Mevcut farklı lisans türlerini öğrenin. Eğer sorunuz varsa,[Aspose satış ekibiyle iletişime geçin](https://about.aspose.com/contact) ve size yardımcı olmaktan mutluluk duyacaklardır.

Her Aspose lisansı, bu süre içinde çıkan tüm yeni sürümlere veya düzeltmelere ücretsiz yükseltmeler için bir yıllık abonelik içerir. Hem lisanslı hem de değerlendirme kullanıcılarına ücretsiz ve sınırsız teknik destek sağlıyoruz.

Lisans, ürün adı, lisanslı geliştirici sayısı, abonelik bitiş tarihi vb. gibi ayrıntıları içeren düz metin bir XML dosyasıdır. Dosya dijital olarak imzalanmıştır, bu nedenle dosyayı değiştirmeyin: dosyaya fazladan bir satır sonu eklemek bile dosyayı geçersiz kılar.
### **Lisans Ne Zaman Uygulanmalı?**
Bu basit kuralları takip edin:

- Lisansın uygulama etki alanı başına yalnızca bir kez ayarlanması gerekir.
- Diğer Aspose.Finance sınıflarını kullanmadan önce lisansı ayarlamanız gerekir.
- SetLicense'i birden çok kez aramak zararlı değildir, ancak işlemci zamanını boşa harcar.
- Bir Windows Forms veya konsol uygulaması geliştiriyorsanız, Aspose.Finance sınıflarını kullanmadan önce başlangıç kodunda SetLicense'i arayın.
- Bir ASP.NET uygulaması geliştirirken, Aplication_Start korumalı yönteminde Global.asax.cs dosyasından SetLicense'i çağırın. Uygulama başladığında bir kez çağrılır.
- SetLicense'i Page_Load metodları içerisinden çağırmayınız çünkü bu, bir web sayfası her yüklendiğinde lisansın da yükleneceği anlamına gelmektedir.
- Bir sınıf kitaplığı geliştiriyorsanız, Aspose.Finance kullanan sınıfın statik oluşturucusundan SetLicense'i çağırırsınız. Statik oluşturucu, Aspose.Finance lisansının doğru şekilde ayarlandığından emin olarak sınıfınızın bir örneği oluşturulmadan önce yürütülür.
### **Dosya veya Akış Nesnesi Kullanarak Lisansı Uygulayın**
 Kullan[Lisans.SetLicense](https://reference.aspose.com/finance/net/aspose.finance/license) bileşeni lisanslama yöntemi. Bir lisans ayarlamanın en kolay yolu, lisans dosyasını Aspose.Finance.dll ile aynı klasöre koymak ve aşağıda gösterildiği gibi dosya adını yolsuz olarak belirtmektir.
#### **Dosyadan Lisans Yükleme**
Bu kod parçacığı, bir dosyada veya katıştırılmış bir kaynakta depolanan bir lisansı başlatır.

```csharp

public static void SetLicenseExample()
{
    // Initialize license object
    Aspose.Finance.License license = new Aspose.Finance.License();
    try
    {
        // Set license
        license.SetLicense("Aspose.Finance.lic");
    }
    catch (Exception)
    {
        // something went wrong
        throw;
    }
    Console.WriteLine("License set successfully.");
}
```
#### **Akış Nesnesinden Lisans Yükleme**
Bu kod parçacıkları, lisansı akıştan başlatır.

```csharp
public static void SetLicenseFromStream()
{
    // Initialize license object
    Aspose.Finance.License license = new Aspose.Finance.License();
    // Load license from the file stream
    System.IO.FileStream myStream =
        new System.IO.FileStream(
            "Aspose.Finance.lic",
            System.IO.FileMode.Open);
    // Set license
    license.SetLicense(myStream);
    Console.WriteLine("License set successfully.");
}
```
## **Tarifeli Lisansı Uygula**
Aspose.Finance for .NET API, geliştiricilerin ölçülü lisans uygulamasına olanak tanır. Yeni bir lisanslama mekanizmasıdır. Yeni lisanslama mekanizması, mevcut lisanslama yöntemiyle birlikte kullanılacaktır. API özelliğinin kullanımına göre faturalandırılmak isteyen müşterilerimiz tarifeli lisanslamayı kullanabilirler. Daha fazla ayrıntı için lütfen bkz.[Ölçülü Lisanslama SSS](https://purchase.aspose.com/faqs/licensing/metered)bölüm.

yeni bir sınıf[ölçülü](https://reference.aspose.com/finance/net/aspose.finance/metered)ölçülü anahtarı uygulamak için eklendi. Bu kod örneği, ölçülü genel ve özel anahtarların nasıl ayarlanacağını gösterir:

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
