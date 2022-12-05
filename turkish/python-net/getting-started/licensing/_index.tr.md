---
title: lisanslama
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /tr/python-net/licensing/
description: Python Finance Kütüphane API müşterilerini Klasik lisans ve Sayaçlı Lisans almaya davet ediyor. Ürünü daha iyi keşfetmek için sınırlı bir lisans kullanmanın yanı sıra.
---
Bazen, sistemi daha iyi incelemek için olabildiğince hızlı bir şekilde koda dalmak istersiniz. Bunu kolaylaştırmak için Aspose.Finance farklı satın alma planları sunar veya değerlendirme için Ücretsiz Deneme ve 30 günlük Geçici Lisans sunar.

{{% alert color="primary" %}}

 Ürünlerimizi nasıl değerlendireceğiniz, uygun şekilde lisanslayacağınız ve satın alacağınız konusunda size rehberlik eden bir dizi genel politika ve uygulama bulunduğunu unutmayın. Onları şurada bulabilirsiniz:["Satın Alma Politikaları ve SSS"](https://purchase.aspose.com/policies) bölüm.

{{% /alert %}}

## **Değerlendir Aspose.Finance**
 Değerlendirme için Aspose.Finance'i kolayca indirebilirsiniz. Değerlendirme paketi, satın alınan paket ile aynıdır. Değerlendirme sürümü, lisansı uygulamak için birkaç satır kod ekledikten sonra kolayca lisanslanır.

### **Değerlendirme Sürümü Sınırlamaları**
Değerlendirme sürümü, aşağıdakiler dışında tüm özellikleri sağlar:

- **Açılan Dosya Sayısı** (Aspose.Finance) Programınızı çalıştırırken Aspose.Finance kütüphanesini kullanarak sadece 50 dosya açabilirsiniz. Uygulamanız bu sayıyı aşarsa bir istisna atılır.
- **Kayıtlı Dosya Sayısı** (Aspose.Finance) Programınızı çalıştırırken Aspose.Finance kütüphanesini kullanarak sadece 50 dosya açabilirsiniz. Uygulamanız bu sayıyı aşarsa bir istisna atılır.

{{% alert color="primary" %}} 

 Aspose.Finance'i değerlendirme kısıtlamaları olmadan denemek istiyorsanız, 30 günlük geçici bir lisans talep edin. Bakınız[Geçici Lisans nasıl alınır?](https://purchase.aspose.com/temporary-license) daha fazla bilgi için.

{{% /alert %}} 

## **Lisans Hakkında**
 Python için Aspose.Finance değerlendirme sürümünü .NET üzerinden kolayca indirebilirsiniz.[indirme sayfası](https://pypi.org/project/aspose.finance/) . Değerlendirme sürümü kesinlikle sağlar**aynı yetenekler**Aspose.Finance'in lisanslı sürümü olarak. Ayrıca, bir lisans satın aldıktan ve lisansı uygulamak için birkaç satır kod ekledikten sonra değerlendirme sürümü kolayca lisanslanır.

Lisans, ürün adı, lisanslandığı geliştiricilerin sayısı, aboneliğin sona erme tarihi gibi ayrıntıları içeren düz metin bir XML dosyasıdır. Dosya dijital olarak imzalanmıştır, bu nedenle dosyayı değiştirmeyin. Dosyanın içeriğine yanlışlıkla fazladan bir satır sonu eklenmesi bile dosyayı geçersiz kılacaktır.

 Değerlendirme sürümüyle ilgili sınırlamalardan kaçınmak için, kullanmadan önce bir lisans ayarlamanız gerekir.**Aspose.Finance**. Uygulama veya işlem başına yalnızca bir kez lisans ayarlamanız gerekir.

## Satın Alınan Lisans

Satın aldıktan sonra lisans dosyasını veya akışını uygulamanız gerekir. Bu bölümde bunun nasıl yapılabileceğine ilişkin seçenekler açıklanmakta ve ayrıca bazı genel sorular hakkında yorumlar yapılmaktadır.

{{% alert color="primary" %}}

Lisansı ayarlamanız gerekir:
* uygulama etki alanı başına yalnızca bir kez
* diğer Aspose.Finance sınıflarını kullanmadan önce

{{% /alert %}}

{{% alert color="primary" %}}

Fiyat bilgisi için fiyat bilgisine ulaşabilirsiniz.["Fiyatlandırma bilgisi"](https://purchase.aspose.com/pricing/finance/family) sayfa.

{{% /alert %}}

### **.NET aracılığıyla Python için Aspose.Finance'de Lisans Ayarlama**

Lisanslar çeşitli konumlardan uygulanabilir:

* Açık yol
* .NET aracılığıyla Python için Aspose.Finance'i çağıran python betiğini içeren klasör
* Aktarım
* Ölçülü Lisans olarak – yeni bir lisanslama mekanizması

{{% alert color="primary" %}}

 Kullan**set_license** bir bileşeni lisanslama yöntemi.

 arama**set_license** birden çok kez zararlı değildir, sadece işlemci zamanını boşa harcar.

{{% /alert %}}

 Aşağıdaki bölümlerde, lisansı ayarlamak için kullanılan iki yaygın yöntemi açıklayacağız.

#### **Dosya Kullanarak Lisans Uygulama**
Bir lisans ayarlamanın en kolay yöntemi, lisans dosyasını Python için Aspose.Finance'i çağıran python betiğini içeren aynı klasöre yerleştirmenizi ve yolu olmadan yalnızca dosya adını belirtmenizi gerektirir.

Bu kod parçacığı, bir lisans dosyası ayarlamak için kullanılır:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

set_license yöntemini çağırırken, lisans adı lisans dosyanızın adı ile aynı olmalıdır. Örneğin, lisans dosyası adını "Aspose.Finance.lic.xml" olarak değiştirebilirsiniz. Ardından, kodunuzda yeni lisans adını (Aspose.Finance.lic.xml) SetLicense yöntemine iletmeniz gerekir.

#### **Akıştan Lisans Uygulama**
 Akıştan bir lisans yükleyebilirsiniz.

Bu kod parçacığı, bir akıştan lisans uygulamak için kullanılır:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Tarifeli Lisansı Uygula

Aspose.Finance, geliştiricilerin ölçülü bir anahtar uygulamasına izin verir. Bu yeni bir lisanslama mekanizmasıdır.

Yeni lisanslama mekanizması, mevcut lisanslama yöntemiyle birlikte kullanılacaktır. API özelliğinin kullanımına göre faturalandırılmak isteyen müşteriler, Tarifeli Lisans kullanabilirler.

 Bu tür bir lisansı almak için gerekli tüm adımları tamamladıktan sonra lisans dosyasını değil anahtarları alacaksınız. Bu ölçülü anahtar kullanılarak uygulanabilir**ölçülü** sınıf, bu amaç için özel olarak tanıtılmıştır.

Aşağıdaki kod örneği, ölçülü genel ve özel anahtarların nasıl ayarlanacağını gösterir:

```py
import aspose.finance as af

# Create an instance of CAD Metered class
metered = af.Metered()

# Access the set_metered_key property and pass public and private keys as parameters
metered.set_metered_key("*****", "*****")

# Get metered data amount before calling API
amountbefore = metered.get_consumption_quantity()
# Display information
print("Amount Consumed Before: " + str(amountbefore))

# handle finance file
# ......

# Get metered data amount After calling API
amountafter = metered.get_consumption_quantity()
# Display information
print("Amount Consumed After: " + str(amountafter))
```

{{% alert color="primary" %}}

 Metered mekanizması doğru hesaplamalar için hizmetlerimizle sürekli etkileşim gerektirdiğinden, Metered lisansının doğru kullanımı için istikrarlı bir İnternet bağlantınızın olması gerektiğini lütfen unutmayın. Daha fazla ayrıntı için bkz.["Ölçümlü Lisanslama SSS"](https://purchase.aspose.com/faqs/licensing/metered) bölüm.

{{% /alert %}}
