---
title: Installation
type: docs
weight: 60
url: /python-net/installation/
description: Learn about Installation of Python Finance Library API using NuGet and Package Manager GUI or Console.
---

## **System Requirements**

First, you have to check and confirm that machine’s specifications meet the [system requirements](/finance/python-net/system-requirements/).

## **Installing Aspose.Finance for Python via .NET**
`pip` is the easiest way to download and install [Aspose.Finance for Python via .NET](https://pypi.org/project/aspose-finance/).

To install Aspose.Finance, run this command: pip install aspose-finance

## **Using Aspose.Finance for Python via .NET**

Once you finish installing the module, you can use Aspose.Finance from your python code this way:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
