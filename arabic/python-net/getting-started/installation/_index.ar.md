---
title: تثبيت
type: docs
weight: 60
url: /ar/python-net/installation/
description: تعرف على تثبيت Python Finance Library API باستخدام NuGet و Package Manager GUI أو Console.
---
## **متطلبات النظام**

 أولاً ، عليك التحقق والتأكد من أن مواصفات الجهاز تفي بـ[متطلبات النظام](/finance/ar/python-net/system-requirements/).

## **تركيب Aspose.Finance لـ Python عبر .NET**
 `pip` هو أسهل طريقة للتنزيل والتثبيت[Aspose.Finance لـ Python عبر .NET](https://pypi.org/project/aspose-finance/).

لتثبيت Aspose.Finance ، قم بتشغيل هذا الأمر: pip install aspose-finance

## **باستخدام Aspose.Finance لـ Python عبر .NET**

بمجرد الانتهاء من تثبيت الوحدة ، يمكنك استخدام Aspose.Finance من كود Python الخاص بك بهذه الطريقة:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
