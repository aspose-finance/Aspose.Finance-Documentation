---
title: 验证Python中的XBRL和iXBRL文件
linktitle: 验证 XBRL 和 iXBRL 文件
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance 库 API 可以验证 XBRL 和 iXBRL 文件。请参阅本文中给出的示例代码以获取更多信息。
type: docs
weight: 30
url: /zh/python-net/validate-xbrl-and-ixbrl-files/
---
## **验证 Python 中的 XBRL 实例文件**
XBRL 实例、XBRL 链接库和 XBRL 分类法模式必须符合[XBRL 规格书](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html).为了验证这些，XbrlInstance 类提供了 validate() 方法。

以下 Python 代码片段演示了如何验证 XBRL 实例文档。

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **验证 Python 中的 iXBRL 文件**
这[iXBRL 规格书](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)定义了许多验证规则。为了验证 iXBRL 文件，InlineXbrlDocument 类提供了一个 validate() 方法。

以下 Python 代码片段演示了验证 iXBRL 实例文档。

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **验证错误代码**
在枚举 ValidationErrorCode 中，为每个验证规则定义了验证错误代码。
以下是错误码定义：

- 语境_时期_不_开始_TIME：上下文期间类型是持续时间，但没有开始日期。
- 语境_时期_不_结尾_TIME：上下文期间类型是持续时间，但没有结束日期。
- 语境_时期_开始_后_END：上下文期间类型为持续时间，但结束日期早于开始日期。
- 语境_立即的_NO_TIME：上下文期间类型是即时的，但没有即时日期。
- 语境_设想_XBRL_NAMESPACE：上下文场景不能有 XBRL 命名空间节点。
- 语境_设想_XBRL_替代_GROUP：上下文场景不能在 XBRL 命名空间中定义的元素的替换组中包含元素。
- 语境_设想_EMPTY：上下文场景不能为空。
- 语境_部分_XBRL_NAMESPACE：上下文段不能有 XBRL 命名空间节点。
- 语境_部分_XBRL_SUBSTITUTIONGROUP：上下文段在 XBRL 命名空间中定义的元素的替换组中不能有元素。
- 语境_部分_EMPTY：上下文段不能为空。
- 物品_不_上下文：项目必须有上下文。
- 物品_长寿_类型_冲突_WITH_CONTEXT：项目的句点类型与上下文冲突。
- 物品_数字_NO_UNIT：项目是数字，必须有一个单位。
- 货币_物品_不_单身的_UNIT_MEASURE：项目是一种货币类型，必须有一个单一的计量单位。
- 货币_物品_NO_ISO4217：项目是货币类型，必须具有 Iso 4217 样式的单位度量。
- 分享_物品_不_单身的_UNIT_MEASURE：项目是一种共享类型，必须有一个单一的单位度量。
- 分享_物品_不_分享_UNIT_MEASURE：项目是共享类型并且必须有一个 xbrli:shares 单位度量。
- 尼尔_物品_和_精确_OR_DECIMALS：项目为零，不得有精度或小数。
- 分数_物品_和_精确_OR_DECIMALS：Item 是分数类型，不能有精度或小数。
- 数字_物品_和_两个都_精确_和_DECIMALS：项目是数字类型，不能同时具有精度和小数。
- 数字_物品_没有_精确_OR_DECIMALS：项目是数字类型，必须有精度或小数。
- 非_数字_物品_和_精确_或者_DECIMALS：项目不是数字类型，不能有精度或小数。
- 脚注_弧_从_不是_已找到：无法从 Loc 中找到脚注弧。
- 脚注_弧_至_不是_已找到：无法找到脚注的脚注弧。
- 定义_弧_从_不是_FOUND：无法从 Loc 找到定义弧。
- 定义_弧_至_不是_FOUND：无法找到 Loc 的定义弧。
- 本质_别名_定义_弧_DIFFERENT_TYPE: Essence-alias 定义弧有不同的类型。
- 本质_别名_定义_弧_不同的_时期_TYPE: Essence-alias Definition arc 有不同的periodTypes。
- 本质_别名_定义_弧_DIFFERENT_BALANCE：本质别名定义弧有不同的平衡。
- 计算_弧_从_不是_FOUND：无法从 Loc 找到计算弧。
- 计算_弧_至_不是_FOUND：无法找到到 Loc 的计算弧。
- 标签_弧_从_不是_FOUND：无法从 Loc 中找到 Lable arc。
- 标签_弧_至_不是_FOUND：无法找到到 Loc 的 Lable 弧。
- 介绍_弧_从_不是_FOUND：无法从 Loc 中找到 Presentation arc。
- 介绍_弧_至_不是_FOUND：无法找到到 Loc 的 Presentation arc。
- 参考_弧_从_不是_FOUND：无法从 Loc 找到参考弧。
- 参考_弧_至_不是_FOUND：无法找到 Loc 的参考弧。
### **标准验证错误消息示例**
![待办事项：图片_替代_文本](validate-xbrl-and-ixbrl-files_1.png)

上面是一个XBRL实例，它定义了context“cd1”，这个context的周期类型是duration，它的开始日期是2002-03-31，结束日期是2001-03-31，所以结束日期早于开始日期。在 XBRL 规范的第 4.7.2 章中，它定义了验证规则：“endDate 必须指定或暗示一个时间点晚于相应 startDate 的指定或暗示时间点”。根据此规则，此 XBRL 实例无效。
## **验证 XBRL 并输出标准错误消息**
以下代码验证 XBRL 实例并输出标准错误消息。

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

下图显示了输出：

![待办事项：图片_替代_文本](validate-xbrl-and-ixbrl-files_2.png)



