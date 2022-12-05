---
title: Installation
type: docs
weight: 60
url: /sv/python-net/installation/
description: Lär dig mer om installation av Python Finance Library API med NuGet och Package Manager GUI eller Console.
---
## **Systemkrav**

 Först måste du kontrollera och bekräfta att maskinens specifikationer uppfyller[Systemkrav](/finance/sv/python-net/system-requirements/).

## **Installerar Aspose.Finance för Python via .NET**
 `pip` är det enklaste sättet att ladda ner och installera[Aspose.Finance för Python via .NET](https://pypi.org/project/aspose-finance/).

För att installera Aspose.Finance, kör detta kommando: pip install aspose-finance

## **Använder Aspose.Finance för Python via .NET**

När du är klar med installationen av modulen kan du använda Aspose.Finance från din pythonkod så här:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
