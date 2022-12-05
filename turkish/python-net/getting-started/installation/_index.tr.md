---
title: Kurulum
type: docs
weight: 60
url: /tr/python-net/installation/
description: Python Finance Kitaplığı API'in NuGet ve Paket Yöneticisi GUI veya Konsolu kullanılarak Kurulumu hakkında bilgi edinin.
---
## **sistem gereksinimleri**

 Öncelikle, makinenin teknik özelliklerinin gereksinimleri karşıladığını kontrol etmeli ve onaylamalısınız.[sistem gereksinimleri](/finance/tr/python-net/system-requirements/).

## **.NET aracılığıyla Python için Aspose.Finance kurulumu**
 `pip`, indirmenin ve kurmanın en kolay yoludur[.NET üzerinden Python için Aspose.Finance](https://pypi.org/project/aspose-finance/).

Aspose.Finance'i yüklemek için şu komutu çalıştırın: pip install aspose-finance

## **.NET aracılığıyla Python için Aspose.Finance'i kullanma**

Modülü kurmayı bitirdikten sonra, python kodunuzdan Aspose.Finance'i şu şekilde kullanabilirsiniz:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
