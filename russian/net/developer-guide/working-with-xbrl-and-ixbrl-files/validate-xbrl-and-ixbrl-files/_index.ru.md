---
title: Проверить файлы XBRL и iXBRL в C#
linktitle: Проверить файлы XBRL и iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance Библиотека API может проверять файлы XBRL и iXBRL. Дополнительные сведения см. в примерах кодов, приведенных в этой статье.
type: docs
weight: 30
url: /ru/net/validate-xbrl-and-ixbrl-files/
---
## **Проверить файл экземпляра XBRL в C#**
 XBRL Экземпляры, XBRL Базы ссылок и XBRL Схемы таксономии ДОЛЖНЫ соответствовать требованиям синтаксиса, установленным в[XBRL спецификация](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Чтобы подтвердить их,[XbrlInstance](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) класс обеспечивает[Подтвердить()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) метод.

В следующем фрагменте кода C# показано, как проверить экземпляр документа XBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **Проверить файл iXBRL в C#**
[iXBRL спецификация](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)определяет множество правил проверки. Для проверки файлов iXBRL[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) класс предоставляет[Подтвердить()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) метод.

Следующий фрагмент кода C# демонстрирует проверку экземпляра документа iXBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Коды ошибок проверки**
 В перечислении[Валидатионерркоде](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) , коды ошибок проверки определяются для каждого правила проверки.
Ниже приведены определения кодов ошибок:

- ContextPeriodNoStartTime: Тип периода контекста — продолжительность, но не имеет даты начала.
- ContextPeriodNoEndTime: Тип периода контекста — продолжительность, но не имеет даты окончания.
- ContextPeriodStartAfterEnd: Тип периода контекста — продолжительность, но дата окончания предшествует дате начала.
- ContextInstantNoTime: тип периода контекста является мгновенным, но не имеет мгновенной даты.
- ContextScenarioXbrlNamespace: сценарий контекста не может иметь узел пространства имен XBRL.
- ContextScenarioXbrlSubstitutionGroup: контекстный сценарий не может иметь элемент в группе подстановки для элементов, определенных в пространстве имен XBRL.
- ContextScenarioEmpty: сценарий контекста не может быть пустым.
- ContextSegmentXbrlNamespace: Сегмент контекста не может иметь узел пространства имен XBRL.
- ContextSegmentXbrlSubstitutionGroup: сегмент контекста не может иметь элемент в группе замены для элементов, определенных в пространстве имен XBRL.
- ContextSegmentEmpty: Сегмент контекста не может быть пустым.
- ItemNoContext: элемент должен иметь контекст.
- ItemPeroidTypeConflictWithContext: у элемента есть конфликт типа периода с контекстом.
- ItemNumericNoUnit: Элемент является числовым и должен иметь единицу измерения.
- MonetaryItemNoSingleUnitMeasure: Элемент является денежным типом и должен иметь единую единицу измерения.
- MonetaryItemNoISO4217: Элемент является денежным типом и должен иметь единицу измерения в стиле Iso 4217.
- ShareItemNoSingleUnitMeasure: элемент относится к типу общего доступа и должен иметь единую меру.
- ShareItemNoShareUnitMeasure: Элемент относится к типу акций и должен иметь единицу измерения xbrli:shares.
- NillItemWithPrecisionOrDecimals: элемент равен нулю и не должен иметь ни точности, ни десятичных знаков.
- FractionItemWithPrecisionOrDecimals: Элемент представляет собой дробный тип и не должен иметь ни точности, ни десятичных знаков.
- NumericItemWithBothPrecisionAndDecimals: элемент является числовым типом и не должен иметь как точность, так и десятичные дроби.
- NumericItemWithoutPrecisionOrDecimals: элемент является числовым типом и должен иметь точность или десятичные дроби.
- NonNumericItemWithPrecisionOrDecimals: элемент не является числовым типом и не должен иметь ни точности, ни десятичных знаков.
- FootnoteArcFromNotFound: невозможно найти дугу сноски из лок.
- FootnoteArcToNotFound: невозможно найти дугу сноски в сноске.
- DefinitionArcFromNotFound: Не удалось найти дугу определения из лок.
- DefinitionArcToNotFound: Не удалось найти дугу определения для местоположения.
- EssenceAliasDefinitionArcDifferentType: дуга определения EssenceAliasDefinitionArcDifferentType имеет разные типы.
- EssenceAliasDefinitionArcDifferentPeriodType: Дуга определения псевдонима сущности имеет разные типы periodTypes.
- EssenceAliasDefinitionArcDifferentBalance: дуга определения EssenceAliasDefinition имеет разные балансы.
- CalculationArcFromNotFound: невозможно найти расчетную дугу из Loc.
- CalculationArcToNotFound: Не удалось найти расчетную дугу для Loc.
- LabelArcFromNotFound: Не удалось найти дугу Lable от Loc.
- LabelArcToNotFound: Не удалось найти дугу Lable, ведущую к Loc.
- PresentationArcFromNotFound: невозможно найти дугу презентации из лок.
- PresentationArcToNotFound: Не удалось найти дугу презентации для местоположения.
- ReferenceArcFromNotFound: Не удалось найти опорную дугу из Loc.
- ReferenceArcToNotFound: Не удалось найти опорную дугу для Loc.
### **Пример стандартного сообщения об ошибке проверки**
![дело:изображение_альтернативный_текст](validate-xbrl-and-ixbrl-files_1.png)

Выше приведен экземпляр XBRL, он определяет контекст «cd1», этот тип периода контекста — продолжительность, его начальная дата — 31 марта 2002 г., дата окончания — 31 марта 2001 г., поэтому дата окончания предшествует дате начала. В спецификации XBRL, глава 4.7.2, определяется правило проверки: «endDate ДОЛЖЕН указывать или подразумевать момент времени, который является более поздним, чем указанный или подразумеваемый момент времени соответствующего startDate». Согласно этому правилу, этот экземпляр XBRL не является допустимым.
## **Подтвердите XBRL и выведите стандартное сообщение об ошибке**
Следующий код проверяет экземпляр XBRL и выводит стандартное сообщение об ошибке.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

На следующем изображении показан результат:

![дело:изображение_альтернативный_текст](validate-xbrl-and-ixbrl-files_2.png)
## **Подтвердите XBRL и выведите индивидуальное сообщение об ошибке.**
Следующий код проверяет экземпляр XBRL и выводит настроенное сообщение об ошибке.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

На следующем изображении показан результат:

![дело:изображение_альтернативный_текст](validate-xbrl-and-ixbrl-files_3.png)

**Подтвердите XBRL и выведите стандартное сообщение об ошибке**


