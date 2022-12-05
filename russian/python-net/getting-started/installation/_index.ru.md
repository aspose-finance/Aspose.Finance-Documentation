---
title: Монтаж
type: docs
weight: 60
url: /ru/python-net/installation/
description: Узнайте об установке библиотеки Python Finance API с помощью NuGet и графического интерфейса или консоли диспетчера пакетов.
---
## **Системные Требования**

 Во-первых, вы должны проверить и подтвердить, что технические характеристики машины соответствуют[Системные Требования](/finance/ru/python-net/system-requirements/).

## **Установка Aspose.Finance на Python через .NET**
 `pip` — самый простой способ скачать и установить[Aspose.Finance для Python через .NET](https://pypi.org/project/aspose-finance/).

Чтобы установить Aspose.Finance, выполните следующую команду: pip install aspose-finance

## **Использование Aspose.Finance для Python через .NET**

Как только вы закончите установку модуля, вы можете использовать Aspose.Finance из своего кода Python следующим образом:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
