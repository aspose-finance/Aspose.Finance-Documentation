---
title: 安装
type: docs
weight: 60
url: /zh/python-net/installation/
description: 了解使用 NuGet 和程序包管理器 GUI 或控制台安装 Python Finance 库 API。
---
## **系统要求**

首先，您必须检查并确认机器的规格符合[系统要求](/finance/zh/python-net/system-requirements/).

## **通过 .NET 为 Python 安装 Aspose.Finance**
 `pip`是最简单的下载安装方式[Aspose.Finance 为 Python 通过 .NET](https://pypi.org/project/aspose-finance/).

要安装 Aspose.Finance，请运行此命令：pip install aspose-finance

## **通过 .NET 将 Aspose.Finance 用于 Python**

完成模块安装后，您可以通过以下方式从 Python 代码中使用 Aspose.Finance：

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
