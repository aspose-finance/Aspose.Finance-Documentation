﻿---
title: 许可
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /zh/net/licensing/
description: C# Finance 图书馆 API 邀请其客户获得经典许可证和计量许可证。以及使用有限许可来更好地探索产品。
---
## **评估 Aspose.Finance**
您可以轻松下载 Aspose.Finance for .NET 产品进行评估。请参阅[Aspose.Finance for .NET 下载页面](https://www.nuget.org/packages/Aspose.Finance/)找出最新版本。评估版提供与许可版组件完全相同的功能。此外，当您添加几行代码来应用许可证时，评估版就会简单地获得许可。

### **评估版限制**
评估版提供除以下功能外的所有功能：

- **打开的文件数**(Aspose.Finance) 运行程序时，使用 Aspose.Finance 库只能打开 50 个文件。如果您的应用程序超过此数量，将抛出异常。
- **保存文件数**(Aspose.Finance) 运行程序时，使用 Aspose.Finance 库只能打开 50 个文件。如果您的应用程序超过此数量，将抛出异常。

{{% alert color="primary" %}} 

如果您想在没有评估限制的情况下试用 Aspose.Finance，请申请 30 天的临时许可证。请参阅[如何获得临时许可证？](https://purchase.aspose.com/temporary-license)了解更多信息。

{{% /alert %}} 
## **申请许可证**
一旦你满意你的[评估](https://downloads.aspose.com/finance/net)Aspose.Finance for .NET，在 Aspose 网站购买许可证：[采购门户](https://purchase.aspose.com/buy).让自己熟悉可用的不同许可证类型。如有任何问题，[联系 Aspose 销售团队](https://about.aspose.com/contact)他们会很乐意帮助你。

每个 Aspose 许可证都包含一年订阅，可以免费升级到在此期间发布的任何新版本或修复程序。我们为许可用户和评估用户提供免费和无限制的技术支持。

许可证是一个纯文本 XML 文件，其中包含产品名称、许可开发人员数量、订阅到期日期等详细信息。该文件经过数字签名，因此请勿修改该文件：即使向该文件添加额外的换行符也会使其无效。
### **何时申请许可证**
遵循这些简单的规则：

- 每个应用程序域只需设置一次许可证。
- 在使用任何其他 Aspose.Finance 类之前，您需要设置许可证。
- 多次调用 SetLicense 没有害处，但会浪费处理器时间。
- 如果您正在开发 Windows 窗体或控制台应用程序，请在启动代码中调用 SetLicense，然后再使用 Aspose.Finance 类。
- 开发 ASP.NET 应用程序时，在 Aplication_Start 保护方法中从 Global.asax.cs 文件调用 SetLicense。它在应用程序启动时被调用一次。
- 不要从 Page_Load 方法中调用 SetLicense，因为这意味着每次加载网页时都会加载许可证。
- 如果您正在开发类库，则从使用 Aspose.Finance 的类的静态构造函数调用 SetLicense。静态构造函数在创建类的实例之前执行，确保正确设置 Aspose.Finance 许可证。
### **使用文件或流对象申请许可证**
使用[许可.SetLicense](https://reference.aspose.com/finance/net/aspose.finance/license)许可组件的方法。设置许可证最简单的方法是将许可证文件放在与 Aspose.Finance.dll 相同的文件夹中，并指定文件名，不带路径，如下所示。
#### **从文件加载许可证**
此代码片段初始化存储在文件或嵌入式资源中的许可证。

```csharp

public static void SetLicenseExample()
{
    // Initialize license object
    Aspose.Finance.License license = new Aspose.Finance.License();
    try
    {
        // Set license
        license.SetLicense("Aspose.Finance.lic");
    }
    catch (Exception)
    {
        // something went wrong
        throw;
    }
    Console.WriteLine("License set successfully.");
}
```
#### **从流对象加载许可证**
这些代码片段从流中初始化许可证。

```csharp
public static void SetLicenseFromStream()
{
    // Initialize license object
    Aspose.Finance.License license = new Aspose.Finance.License();
    // Load license from the file stream
    System.IO.FileStream myStream =
        new System.IO.FileStream(
            "Aspose.Finance.lic",
            System.IO.FileMode.Open);
    // Set license
    license.SetLicense(myStream);
    Console.WriteLine("License set successfully.");
}
```
## **应用计量许可证**
Aspose.Finance for .NET API 允许开发人员应用计量许可证。这是一种新的许可机制。新的许可机制将与现有的许可方法一起使用。那些希望根据 API 功能的使用情况进行计费的客户可以使用计量许可。详情请参阅[计量许可常见问题解答](https://purchase.aspose.com/faqs/licensing/metered)部分。

一个新班级[计量的](https://reference.aspose.com/finance/net/aspose.finance/metered)已添加以应用计量密钥。此代码示例演示如何设置计量公钥和私钥：

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
