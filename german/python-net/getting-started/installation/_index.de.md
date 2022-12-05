---
title: Installation
type: docs
weight: 60
url: /de/python-net/installation/
description: Erfahren Sie mehr über die Installation von Python Finance Library API unter Verwendung von NuGet und Package Manager GUI oder Console.
---
## **System Anforderungen**

 Zuerst müssen Sie überprüfen und bestätigen, dass die Spezifikationen der Maschine den entsprechen[System Anforderungen](/finance/de/python-net/system-requirements/).

## **Installieren von Aspose.Finance für Python über .NET**
 `pip` ist der einfachste Weg zum Herunterladen und Installieren[Aspose.Finance für Python über .NET](https://pypi.org/project/aspose-finance/).

Um Aspose.Finance zu installieren, führen Sie diesen Befehl aus: pip install aspose-finance

## **Verwenden Sie Aspose.Finance für Python über .NET**

Sobald Sie die Installation des Moduls abgeschlossen haben, können Sie Aspose.Finance auf diese Weise aus Ihrem Python-Code verwenden:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
