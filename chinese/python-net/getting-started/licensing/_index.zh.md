---
title: 许可
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /zh/python-net/licensing/
description: Python Finance 图书馆 API 邀请其客户获得经典许可证和计量许可证。以及使用有限许可来更好地探索产品。
---
有时，为了更好地研究系统，你想尽快深入代码。为了使这更容易，Aspose.Finance 提供不同的购买计划或提供免费试用和 30 天的临时许可证以供评估。

{{% alert color="primary" %}}

请注意，有许多一般政策和惯例可指导您如何评估、正确许可和购买我们的产品。您可以在[“购买政策和常见问题解答”](https://purchase.aspose.com/policies)部分。

{{% /alert %}}

## **评估 Aspose.Finance**
您可以轻松下载 Aspose.Finance 进行评估。评估包与购买包相同。在您添加几行代码以应用许可证后，评估版便会获得许可。

### **评估版限制**
评估版提供除以下功能外的所有功能：

- **打开的文件数**(Aspose.Finance) 运行程序时，使用 Aspose.Finance 库只能打开 50 个文件。如果您的应用程序超过此数量，将抛出异常。
- **保存文件数**(Aspose.Finance) 运行程序时，使用 Aspose.Finance 库只能打开 50 个文件。如果您的应用程序超过此数量，将抛出异常。

{{% alert color="primary" %}} 

如果您想在没有评估限制的情况下试用 Aspose.Finance，请申请 30 天的临时许可证。请参阅[如何获得临时许可证？](https://purchase.aspose.com/temporary-license)了解更多信息。

{{% /alert %}} 

## **关于许可证**
您可以通过 .NET 从其轻松下载 Aspose.Finance 的评估版 Python[下载页面](https://pypi.org/project/aspose.finance/).评估版提供绝对**相同的能力**作为 Aspose.Finance 的许可版本。此外，在您购买许可证并添加几行代码以应用许可证后，评估版将成为许可版本。

该许可证是一个纯文本 XML 文件，其中包含产品名称、获得许可的开发人员数量、订阅到期日期等详细信息。该文件经过数字签名，因此请勿修改该文件。即使无意中在文件内容中添加了额外的换行符也会使其无效。

为避免与评估版相关的限制，您需要在使用前设置许可证**Aspose.Finance**.您只需为每个应用程序或进程设置一次许可证。

## 购买的许可证

购买后，您需要申请许可证文件或流。本节描述如何完成此操作的选项，以及对一些常见问题的评论。

{{% alert color="primary" %}}

您需要设置许可证：
* 每个应用程序域仅一次
在使用任何其他 Aspose.Finance 类之前

{{% /alert %}}

{{% alert color="primary" %}}

您可以在[“定价信息”](https://purchase.aspose.com/pricing/finance/family)页。

{{% /alert %}}

### **通过 .NET 在 Aspose.Finance 中为 Python 设置许可证**

可以从不同位置应用许可证：

* 显式路径
包含通过 .NET 为 Python 调用 Aspose.Finance 的 python 脚本的文件夹
溪流
作为计量许可——一种新的许可机制

{{% alert color="primary" %}}

使用**设置许可证**许可组件的方法。

呼唤**设置许可证**多次是无害的，它只是浪费处理器时间。

{{% /alert %}}

在下面的部分中，我们将描述用于设置许可证的两种常用方法。

#### **使用文件应用许可证**
设置许可证的最简单方法要求您将许可证文件放在包含为 Python 调用 Aspose.Finance 的 python 脚本的同一文件夹中，并仅指定文件名而不指定其路径。

此代码段用于设置许可证文件：

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

调用 set_license 方法时，许可证名称应与您的许可证文件相同。例如，您可以将许可证文件名更改为“Aspose.Finance.lic.xml”。然后，在您的代码中，您必须将新的许可证名称 (Aspose.Finance.lic.xml) 传递给 SetLicense 方法。

#### **从流中应用许可证**
您可以从流中加载许可证。

此代码片段用于从流中应用许可证：

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### 应用计量许可证

Aspose.Finance 允许开发人员应用计量密钥。这是一种新的许可机制。

新的许可机制将与现有的许可方法一起使用。那些希望根据 API 功能的使用进行计费的客户可以使用计量许可。

完成获得此类许可证的所有必要步骤后，您将收到密钥，而不是许可证文件。这个计量密钥可以使用**计量的**为此专门引入的类。

以下代码示例显示如何设置计量公钥和私钥：

```py
import aspose.finance as af

# Create an instance of CAD Metered class
metered = af.Metered()

# Access the set_metered_key property and pass public and private keys as parameters
metered.set_metered_key("*****", "*****")

# Get metered data amount before calling API
amountbefore = metered.get_consumption_quantity()
# Display information
print("Amount Consumed Before: " + str(amountbefore))

# handle finance file
# ......

# Get metered data amount After calling API
amountafter = metered.get_consumption_quantity()
# Display information
print("Amount Consumed After: " + str(amountafter))
```

{{% alert color="primary" %}}

请注意，您必须拥有稳定的互联网连接才能正确使用计量许可证，因为计量机制需要与我们的服务持续交互才能进行正确计算。有关详细信息，请参阅[“计量许可常见问题解答”](https://purchase.aspose.com/faqs/licensing/metered)部分。

{{% /alert %}}
