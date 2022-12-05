---
title: 验证C#中的XBRL和iXBRL文件
linktitle: 验证 XBRL 和 iXBRL 文件
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance 库 API 可以验证 XBRL 和 iXBRL 文件。请参阅本文中给出的示例代码以获取更多信息。
type: docs
weight: 30
url: /zh/net/validate-xbrl-and-ixbrl-files/
---
## **验证 C# 中的 XBRL 实例文件**
XBRL 实例、XBRL 链接库和 XBRL 分类法模式必须符合[XBRL 规格书](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html).为了验证这些，[Xbrl实例](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance)类提供了[证实（）](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate)方法。

以下 C# 代码片段演示了如何验证 XBRL 实例文档。

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **验证 C# 中的 iXBRL 文件**
这[iXBRL 规格书](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)定义了许多验证规则。为了验证 iXBRL 文件，[内联Xbrl文档](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument)类提供了[证实（）](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate)方法。

以下 C# 代码片段演示了验证 iXBRL 实例文档。

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **验证错误代码**
在枚举中[验证错误代码](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode)，为每个验证规则定义了验证错误代码。
以下是错误码定义：

- ContextPeriodNoStartTime：上下文周期类型是持续时间，但没有开始日期。
- ContextPeriodNoEndTime：上下文期间类型是持续时间，但没有结束日期。
- ContextPeriodStartAfterEnd：上下文期间类型为持续时间，但结束日期早于开始日期。
- ContextInstantNoTime：上下文期间类型是即时的，但没有即时日期。
- ContextScenarioXbrlNamespace：上下文场景不能有 XBRL 命名空间节点。
- ContextScenarioXbrlSubstitutionGroup：上下文场景在 XBRL 命名空间中定义的元素的替换组中不能有元素。
- ContextScenarioEmpty：上下文场景不能为空。
- ContextSegmentXbrlNamespace：上下文段不能有 XBRL 命名空间节点。
- ContextSegmentXbrlSubstitutionGroup：上下文段在 XBRL 命名空间中定义的元素的替换组中不能有元素。
- ContextSegmentEmpty：上下文段不能为空。
- ItemNoContext：项目必须有上下文。
- ItemPeroidTypeConflictWithContext：项目的句点类型与上下文冲突。
- ItemNumericNoUnit：项目是数字，必须有一个单位。
- MonetaryItemNoSingleUnitMeasure：Item 是一种货币类型，必须有一个单一的计量单位。
- MonetaryItemNoISO4217：项目是一种货币类型，必须具有 Iso 4217 样式的单位度量。
- ShareItemNoSingleUnitMeasure：Item 是一个共享类型，必须有一个单一的单位度量。
- ShareItemNoShareUnitMeasure：项目是共享类型并且必须具有 xbrli:shares 单位度量。
- NillItemWithPrecisionOrDecimals：项目为 nil，不得有精度或小数。
- FractionItemWithPrecisionOrDecimals：项目是分数类型，不能有精度或小数。
- NumericItemWithBothPrecisionAndDecimals：项目是数字类型，不能同时具有精度和小数。
- NumericItemWithoutPrecisionOrDecimals：项目是数字类型，必须具有精度或小数。
- NonNumericItemWithPrecisionOrDecimals：项目不是数字类型，不能有精度或小数。
- FootnoteArcFromNotFound：无法从 Loc 找到脚注弧。
- FootnoteArcToNotFound：无法找到到脚注的脚注弧。
- DefinitionArcFromNotFound：无法从 Loc 找到定义弧。
- DefinitionArcToNotFound：无法找到到 Loc 的定义弧。
- EssenceAliasDefinitionArcDifferentType: Essence-alias Definition arc有不同的类型。
- EssenceAliasDefinitionArcDifferentPeriodType: Essence-alias Definition arc 有不同的periodTypes。
- EssenceAliasDefinitionArcDifferentBalance：本质别名定义弧有不同的平衡。
- CalculationArcFromNotFound：无法从 Loc 找到计算弧。
- CalculationArcToNotFound：无法找到 Loc 的计算弧。
- LabelArcFromNotFound：无法从 Loc 找到 Lable 弧。
- LabelArcToNotFound：无法找到到 Loc 的 Lable 弧。
- PresentationArcFromNotFound：无法从 Loc 中找到 Presentation arc。
- PresentationArcToNotFound：无法找到到 Loc 的 Presentation arc。
- ReferenceArcFromNotFound：无法从 Loc 找到参考弧。
- ReferenceArcToNotFound：无法找到 Loc 的参考弧。
### **标准验证错误消息示例**
![待办事项：图片_替代_文本](validate-xbrl-and-ixbrl-files_1.png)

上面是一个XBRL实例，它定义了context“cd1”，这个context的周期类型是duration，它的开始日期是2002-03-31，结束日期是2001-03-31，所以结束日期早于开始日期。在 XBRL 规范的第 4.7.2 章中，它定义了验证规则：“endDate 必须指定或暗示一个时间点晚于相应 startDate 的指定或暗示时间点”。根据此规则，此 XBRL 实例无效。
## **验证 XBRL 并输出标准错误消息**
以下代码验证 XBRL 实例并输出标准错误消息。

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

下图显示了输出：

![待办事项：图片_替代_文本](validate-xbrl-and-ixbrl-files_2.png)
## **验证 XBRL 并输出自定义错误消息**
以下代码验证 XBRL 实例并输出自定义错误消息。

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

下图显示了输出：

![待办事项：图片_替代_文本](validate-xbrl-and-ixbrl-files_3.png)

**验证 XBRL 并输出标准错误消息**


