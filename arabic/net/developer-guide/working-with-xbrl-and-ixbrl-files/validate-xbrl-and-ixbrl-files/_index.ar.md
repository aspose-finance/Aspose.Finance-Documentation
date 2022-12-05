---
title: تحقق من صحة ملفات XBRL و iXBRL في C#
linktitle: تحقق من صحة ملفات XBRL و iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance مكتبة API يمكنها التحقق من صحة ملفات XBRL و iXBRL. يرجى الاطلاع على نماذج الرموز الواردة في هذه المقالة لمزيد من المعلومات.
type: docs
weight: 30
url: /ar/net/validate-xbrl-and-ixbrl-files/
---
## **تحقق من صحة ملف المثيل XBRL في C#**
 يجب أن تتوافق مثيلات XBRL و XBRL Linkbases و XBRL مخططات التصنيف مع متطلبات بناء الجملة المفروضة في[مواصفات XBRL](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). للتحقق من صحة هذه ، فإن[XbrlInstance](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) فئة توفر[التحقق من صحة ()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) طريقة.

يوضح مقتطف التعليمات البرمجية C# التالي كيفية التحقق من صحة مستند مثيل XBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **تحقق من صحة الملف iXBRL في C#**
 ال[مواصفات iXBRL](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)يحدد العديد من قواعد التحقق من الصحة. للتحقق من صحة ملفات iXBRL ، فإن ملف[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) فئة توفر أ[التحقق من صحة ()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) طريقة.

يوضح مقتطف التعليمات البرمجية C# التالي التحقق من صحة وثيقة نسخة iXBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **أكواد خطأ التحقق من الصحة**
 في التعداد[ValidationErrorCode](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) ، يتم تحديد رموز خطأ التحقق من الصحة لكل قاعدة من قواعد التحقق من الصحة.
فيما يلي تعريفات رمز الخطأ:

- ContextPeriodNoStartTime: نوع فترة السياق هي المدة ، ولكن ليس لها تاريخ بدء.
- ContextPeriodNoEndTime: نوع فترة السياق هي المدة ، ولكن ليس لها تاريخ انتهاء.
- ContextPeriodStartAfterEnd: نوع فترة السياق هي المدة ، ولكن تاريخ الانتهاء يسبق تاريخ البدء.
- ContextInstantNoTime: نوع فترة السياق فوري ، ولكن ليس له تاريخ فوري.
- ContextScenarioXbrlNamespace: لا يمكن أن يحتوي سيناريو السياق على XBRL عقدة مساحة الاسم.
- ContextScenarioXbrlSubstitutionGroup: لا يمكن أن يحتوي سيناريو السياق على عنصر في مجموعة الاستبدال للعناصر المحددة في مساحة الاسم XBRL.
- ContextScenarioEmpty: لا يمكن أن يكون سيناريو السياق فارغًا.
- ContextSegmentXbrlNamespace: لا يمكن أن تحتوي قطعة السياق على XBRL عقدة مساحة الاسم.
- ContextSegmentXbrlSubstitutionGroup: لا يمكن أن يحتوي مقطع السياق على عنصر في مجموعة الاستبدال للعناصر المحددة في مساحة الاسم XBRL.
- ContextSegmentEmpty: لا يمكن أن يكون مقطع السياق فارغًا.
- ItemNoContext: يجب أن يكون للعنصر سياق.
- ItemPeroidTypeConflictWithContext: يحتوي العنصر على نوع فترة يتعارض مع السياق.
- ItemNumericNoUnit: العنصر رقمي ويجب أن يحتوي على وحدة.
- MonetaryItemNoSingleUnitMeasure: العنصر هو نوع نقدي ويجب أن يحتوي على وحدة قياس واحدة.
- MonetaryItemNoISO4217: العنصر هو نوع نقدي ويجب أن يحتوي على مقياس وحدة نمط Iso 4217.
- ShareItemNoSingleUnitMeasure: العنصر هو نوع مشاركة ويجب أن يحتوي على وحدة قياس واحدة.
- ShareItemNoShareUnitMeasure: العنصر هو نوع المشاركة ويجب أن يكون له xbrli: قياس وحدة الأسهم.
- NillItemWithPrecisionOrDecimals: العنصر لا شيء ويجب ألا يحتوي على دقة أو كسور عشرية.
- FractionItemWithPrecisionOrDecimals: العنصر هو نوع كسر ويجب ألا يحتوي على دقة أو كسور عشرية.
- NumericItemWithBothPrecisionAndDecimals: العنصر هو نوع رقمي ويجب ألا يحتوي على كل من الدقة والأرقام العشرية.
- NumericItemWithoutPrecisionOrDecimals: العنصر هو نوع رقمي ويجب أن يحتوي إما على الدقة أو الكسور العشرية.
- NonNumericItemWithPrecisionOrDecimals: العنصر ليس نوعًا رقميًا ويجب ألا يحتوي على دقة أو كسور عشرية.
- FootnoteArcFromNotFound: تعذر العثور على قوس الحاشية السفلية من Loc.
- FootnoteArcToNotFound: تعذر العثور على قوس حاشية سفلية إلى حاشية سفلية.
- DefinitionArcFromNotFound: تعذر العثور على قوس التعريف من Loc.
- DefinitionArcToNotFound: تعذر العثور على تعريف القوس لـ Loc.
- EssenceAliasDefinitionArcDifferentType: Essence-alias تعريف القوس له أنواع مختلفة.
- EssenceAliasDefinitionArcDifferentPeriodType: Essence-alias تعريف القوس له أنواع مختلفة من periodTypes.
- EssenceAliasDefinitionArcDifferentBalance: Essence-alias تعريف القوس له أرصدة مختلفة.
- CalculationArcFromNotFound: تعذر العثور على قوس الحساب من Loc.
- CalculationArcToNotFound: تعذر العثور على قوس الحساب إلى Loc.
- LabelArcFromNotFound: تعذر العثور على قوس Lable من Loc.
- LabelArcToNotFound: تعذر العثور على قوس Lable إلى Loc.
- PresentationArcFromNotFound: تعذر العثور على قوس عرض تقديمي من Loc.
- PresentationArcToNotFound: تعذر العثور على قوس عرض تقديمي إلى Loc.
- ReferenceArcFromNotFound: تعذر العثور على قوس مرجعي من Loc.
- ReferenceArcToNotFound: تعذر العثور على قوس مرجعي لـ Loc.
### **مثال على رسالة خطأ التحقق القياسية**
![ما يجب القيام به: image_بديل_نص](validate-xbrl-and-ixbrl-files_1.png)

أعلاه هو مثيل XBRL ، فهو يعرّف السياق "cd1" ، ونوع فترة السياق هذا هو المدة ، وتاريخ البدء هو 2002-03-31 ، وتاريخ الانتهاء هو 31-03-2001 ، لذلك يكون تاريخ الانتهاء قبل تاريخ البدء. في مواصفة XBRL ، الفصل 4.7.2 ، تحدد قاعدة التحقق من الصحة: "يجب أن يحدد تاريخ الانتهاء أو يشير إلى نقطة زمنية بعد النقطة المحددة أو الضمنية في وقت تاريخ البدء المقابل". وفقًا لهذه القاعدة ، لا يعد مثيل XBRL هذا صالحًا.
## **تحقق من صحة XBRL وإخراج رسالة الخطأ المعيارية**
يقوم الكود التالي بالتحقق من صحة مثيل XBRL وإخراج رسالة الخطأ القياسية.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

الصورة التالية توضح الإخراج:

![ما يجب القيام به: image_بديل_نص](validate-xbrl-and-ixbrl-files_2.png)
## **قم بالتحقق من صحة XBRL وإخراج رسالة الخطأ المخصصة**
تقوم التعليمات البرمجية التالية بالتحقق من صحة مثيل XBRL وإخراج رسالة خطأ مخصصة.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

الصورة التالية توضح الإخراج:

![ما يجب القيام به: image_بديل_نص](validate-xbrl-and-ixbrl-files_3.png)

**تحقق من صحة XBRL وإخراج رسالة الخطأ المعيارية**


