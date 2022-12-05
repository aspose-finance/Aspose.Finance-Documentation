---
title: الترخيص
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /ar/net/licensing/
description: C# Finance المكتبة API تدعو عملائها للحصول على رخصة كلاسيكية ورخصة عداد. بالإضافة إلى استخدام ترخيص محدود لاستكشاف المنتج بشكل أفضل.
---
## **أوجد Aspose.Finance**
يمكنك بسهولة تنزيل Aspose.Finance for .NET المنتج لأغراض التقييم. يرجى الرجوع إلى[Aspose.Finance for .NET صفحة التحميل](https://www.nuget.org/packages/Aspose.Finance/)لمعرفة أحدث إصدار. يوفر الإصدار التقييمي نفس الإمكانات تمامًا مثل الإصدار المرخص من المكون. علاوة على ذلك ، يصبح الإصدار التقييمي مرخصًا ببساطة عند إضافة بضعة أسطر من التعليمات البرمجية لتطبيق الترخيص.

### **قيود إصدار التقييم**
يوفر الإصدار التقييمي جميع الميزات باستثناء ما يلي:

- **عدد الملفات المفتوحة** (Aspose.Finance) عند تشغيل البرنامج ، يمكنك فقط فتح 50 ملفًا باستخدام مكتبة Aspose.Finance. إذا تجاوز التطبيق الخاص بك هذا الرقم ، فسيتم طرح استثناء.
- **عدد الملفات المحفوظة** (Aspose.Finance) عند تشغيل البرنامج ، يمكنك فقط فتح 50 ملفًا باستخدام مكتبة Aspose.Finance. إذا تجاوز التطبيق الخاص بك هذا الرقم ، فسيتم طرح استثناء.

{{% alert color="primary" %}} 

 إذا كنت تريد تجربة Aspose.Finance بدون قيود تقييم ، فاطلب ترخيصًا مؤقتًا لمدة 30 يومًا. يرجى الرجوع إلى[كيف تحصل على رخصة مؤقتة؟](https://purchase.aspose.com/temporary-license) للمزيد من المعلومات.

{{% /alert %}} 
## **طلب ترخيص**
 بمجرد أن تصبح سعيدًا بملف[تقييم](https://downloads.aspose.com/finance/net) من Aspose.Finance for .NET ، قم بشراء ترخيص على موقع الويب Aspose:[بوابة الشراء](https://purchase.aspose.com/buy) تعرف على أنواع التراخيص المختلفة المتاحة. إذا كان لديك أية أسئلة،[اتصل بفريق المبيعات Aspose](https://about.aspose.com/contact) وسيسعدهم مساعدتك.

يحمل كل ترخيص Aspose اشتراكًا لمدة عام واحد للترقيات المجانية لأي إصدارات جديدة أو إصلاحات تظهر خلال هذا الوقت. نحن نقدم دعمًا فنيًا مجانيًا وغير محدود لكل من المستخدمين المرخصين والمستخدمين المقيّمين.

الترخيص عبارة عن ملف XML نص عادي يحتوي على تفاصيل مثل اسم المنتج وعدد المطورين المرخصين وتاريخ انتهاء الاشتراك وما إلى ذلك. الملف موقّع رقميًا ، لذا لا تقم بتعديل الملف: حتى إضافة فاصل أسطر إضافي إلى الملف يبطله.
### **متى يتم تطبيق الترخيص**
اتبع هذه القواعد البسيطة:

- يلزم تعيين الترخيص مرة واحدة فقط لكل مجال تطبيق.
- تحتاج إلى تعيين الترخيص قبل استخدام أي فئات Aspose.Finance أخرى.
- لا يعد استدعاء SetLicense عدة مرات ضارًا ، ولكنه يضيع وقت المعالج.
- إذا كنت تقوم بتطوير Windows Forms أو تطبيق وحدة التحكم ، فاتصل بـ SetLicense في كود بدء التشغيل ، قبل استخدام فئات Aspose.Finance.
- عند تطوير تطبيق ASP.NET ، قم باستدعاء SetLicense من الملف Global.asax.cs ، في أسلوب Aplication_Start المحمي. يتم استدعاؤه مرة واحدة عند بدء التطبيق.
- لا تستدعي SetLicense من داخل طرق Page_Load حيث أن ذلك يعني أن الترخيص سيتم تحميله في كل مرة يتم فيها تحميل صفحة ويب.
- إذا كنت تقوم بتطوير مكتبة فئة ، يمكنك استدعاء SetLicense من مُنشئ ثابت للفئة التي تستخدم Aspose.Finance. يتم تنفيذ المُنشئ الثابت قبل إنشاء مثيل للفئة الخاصة بك مع التأكد من تعيين ترخيص Aspose.Finance بشكل صحيح.
### **تطبيق الترخيص باستخدام ملف أو كائن دفق**
 استخدم ال[الترخيص](https://reference.aspose.com/finance/net/aspose.finance/license) طريقة لترخيص المكون. أسهل طريقة لتعيين ترخيص هي وضع ملف الترخيص في نفس المجلد مثل Aspose.Finance.dll وتحديد اسم الملف ، بدون مسار ، كما هو موضح أدناه.
#### **تحميل ترخيص من ملف**
يقوم مقتطف الشفرة هذا بتهيئة ترخيص مخزن في ملف أو في مورد مضمن.

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
#### **تحميل ترخيص من كائن تيار**
تعمل مقتطفات التعليمات البرمجية هذه على تهيئة الترخيص من الدفق.

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
## **تطبيق الترخيص المقنن**
Aspose.Finance for .NET API يسمح للمطورين بتطبيق الترخيص المقنن. إنها آلية ترخيص جديدة. سيتم استخدام آلية الترخيص الجديدة جنبًا إلى جنب مع طريقة الترخيص الحالية. يمكن للعملاء الذين يرغبون في دفع فواتيرهم بناءً على استخدام ميزات API استخدام الترخيص المقنن. لمزيد من التفاصيل ، يرجى الرجوع إلى[الأسئلة الشائعة حول الترخيص المقنن](https://purchase.aspose.com/faqs/licensing/metered)الجزء.

فئة جديدة[مقننة](https://reference.aspose.com/finance/net/aspose.finance/metered)تمت إضافته لتطبيق المفتاح المقنن. يوضح مثال الرمز هذا كيفية تعيين المفاتيح العامة والخاصة التي تم قياسها:

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
