---
title: XBRL ve iXBRL dosyalarını C#'de doğrulayın
linktitle: XBRL ve iXBRL dosyalarını doğrulayın
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance Kütüphane API, XBRL ve iXBRL dosyalarını doğrulayabilir. Daha fazla bilgi için lütfen bu makalede verilen örnek kodlara bakın.
type: docs
weight: 30
url: /tr/net/validate-xbrl-and-ixbrl-files/
---
## **XBRL örnek dosyasını C#'de doğrulayın**
 XBRL Bulut Sunucuları, XBRL Bağlantı Tabanları ve XBRL Taksonomi Şemaları, belirtilen sözdizimi gereksinimlerine UYMALIDIR[XBRL spesifikasyonu](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Bunları doğrulamak için,[Xbrl Örneği](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) sınıf sağlar[Doğrula()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) yöntem.

Aşağıdaki C# kod parçacığı, bir XBRL örnek belgesinin nasıl doğrulanacağını gösterir.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **iXBRL dosyasını C#'de doğrula**
 bu[iXBRL spesifikasyonu](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)birçok doğrulama kuralı tanımlar. iXBRL dosyalarını doğrulamak için,[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) sınıf bir sağlar[Doğrula()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) yöntem.

Aşağıdaki C# kod parçacığı, bir iXBRL örnek belgesinin doğrulanmasını gösterir.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Doğrulama hata kodları**
 numaralandırmada[ValidationErrorCode](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) , her doğrulama kuralı için doğrulama hata kodları tanımlanır.
Hata kodu tanımları aşağıdadır:

- ContextPeriodNoStartTime: Bağlam periyodu tipi süredir, ancak başlangıç tarihi yoktur.
- ContextPeriodNoEndTime: Bağlam dönemi türü süre, ancak bitiş tarihi yok.
- ContextPeriodStartAfterEnd: Bağlam dönemi türü süre, ancak bitiş tarihi başlangıç tarihinden önce.
- ContextInstantNoTime: Bağlam dönemi türü anlıktır, ancak anlık tarihi yoktur.
- ContextScenarioXbrlNamespace: Bağlam senaryosunda XBRL ad alanı düğümü olamaz.
- ContextScenarioXbrlSubstitutionGroup: Bağlam senaryosu, XBRL ad alanında tanımlanan öğeler için ikame grubunda bir öğeye sahip olamaz.
- ContextScenarioEmpty: Bağlam senaryosu boş olamaz.
- ContextSegmentXbrlNamespace: Bağlam segmenti XBRL ad alanı düğümüne sahip olamaz.
- ContextSegmentXbrlSubstitutionGroup: Bağlam segmenti, XBRL ad alanında tanımlanan öğeler için ikame grubunda öğeye sahip olamaz.
- ContextSegmentEmpty: Bağlam segmenti boş olamaz.
- ItemNoContext: Öğenin bir bağlamı olmalıdır.
- ItemPeroidTypeConflictWithContext: Öğenin bağlamla dönem türü çakışması var.
- ItemNumericNoUnit: Öğe sayısaldır ve bir birimi olmalıdır.
- MonetaryItemNoSingleUnitMeasure: Öğe parasal bir türdür ve tek bir birim ölçüsü olmalıdır.
- MonetaryItemNoISO4217: Öğe, parasal bir türdür ve Iso 4217 stil birim ölçüsüne sahip olmalıdır.
- ShareItemNoSingleUnitMeasure: Öğe bir paylaşım türüdür ve tek bir birim ölçüsü olmalıdır.
- ShareItemNoShareUnitMeasure: Öğe, paylaşım türüdür ve bir xbrli:shares birim ölçüsüne sahip olmalıdır.
- NillItemWithPrecisionOrDecimals: Öğe sıfırdır ve kesinliği veya ondalık sayıları olmamalıdır.
- FractionItemWithPrecisionOrDecimals: Öğe bir kesir türüdür ve kesinliği veya ondalık sayıları olmamalıdır.
- NumericItemWithBothPrecisionAndDecimals: Öğe, sayısal bir türdür ve hem duyarlılığa hem de ondalık sayılara sahip olmamalıdır.
- NumericItemWithoutPrecisionOrDecimals: Öğe sayısal bir türdür ve kesinliği veya ondalık sayıları olmalıdır.
- NonNumericItemWithPrecisionOrDecimals: Öğe sayısal bir tür değildir ve kesinliği veya ondalık sayıları olmamalıdır.
- FootnoteArcFromNotFound: Loc'tan Dipnot yayı bulunamadı.
- FootnoteArcToNotFound: Dipnottan Dipnota geçiş bulunamıyor.
- DefinitionArcFromNotFound: Loc'tan Tanım yayı bulunamadı.
- DefinitionArcToNotFound: Loc için Tanım yayı bulunamadı.
- EssenceAliasDefinitionArcDifferentType: Essence-alias Tanım arc'ın farklı türleri vardır.
- EssenceAliasDefinitionArcDifferentPeriodType: Essence-alias Tanım arc'ın farklı periodType'ları vardır.
- EssenceAliasDefinitionArcDifferentBalance: Essence-alias Tanım arkın farklı dengeleri vardır.
- CalculationArcFromNotFound: Loc'tan Hesaplama yayı bulunamadı.
- CalculationArcToNotFound: Loc için Hesaplama yayı bulunamadı.
- LabelArcFromNotFound: Loc'tan Lable yayı bulunamadı.
- LabelArcToNotFound: Loc'a etiket yayı bulunamadı.
- PresentationArcFromNotFound: Loc'tan bir Sunum yayı bulunamadı.
- PresentationArcToNotFound: Loc için bir Sunum yayı bulunamadı.
- ReferenceArcFromNotFound: Loc'tan bir Referans yayı bulunamadı.
- ReferenceArcToNotFound: Loc için bir Referans yayı bulunamadı.
### **Standart doğrulama hata mesajı örneği**
![yapılacaklar:resim_alternatif_Metin](validate-xbrl-and-ixbrl-files_1.png)

Yukarıdaki bir XBRL örneğidir, “cd1” bağlamını tanımlar, bu bağlam periyodu türü süre, başlangıç tarihi 2002-03-31, bitiş tarihi 2001-03-31, yani bitiş tarihi başlangıç tarihinden önce. XBRL spesifikasyonu, bölüm 4.7.2'de doğrulama kuralını tanımlar: "bitişTarihi, ilgili başlangıçTarihi'nin belirtilen veya ima edilen zamanından daha sonra olan bir zaman noktasını belirtmeli veya ima etmelidir". Bu kurala göre, bu XBRL örneği geçerli değil.
## **XBRL'i doğrulayın ve standart hata mesajı alın**
Aşağıdaki kod, XBRL örneğini doğrular ve standart hata mesajını verir.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

Aşağıdaki görüntü çıktıyı gösterir:

![yapılacaklar:resim_alternatif_Metin](validate-xbrl-and-ixbrl-files_2.png)
## **XBRL'i doğrulayın ve özelleştirilmiş hata mesajının çıktısını alın**
Aşağıdaki kod, XBRL örneğini doğrular ve özelleştirilmiş hata mesajı verir.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

Aşağıdaki görüntü çıktıyı gösterir:

![yapılacaklar:resim_alternatif_Metin](validate-xbrl-and-ixbrl-files_3.png)

**XBRL'i doğrulayın ve standart hata mesajı alın**


