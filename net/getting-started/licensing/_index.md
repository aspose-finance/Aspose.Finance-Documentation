---
title: Licensing
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /net/licensing/
description: C# Finance Library API invites its customers to get a Classic license and Metered License. As well as use a limited license to better explore the product.
---

## **Evaluate Aspose.Finance**
You can easily download Aspose.Finance for .NET product for evaluation purposes. Please refer to the [Aspose.Finance for .NET download page](https://www.nuget.org/packages/Aspose.Finance/) to find out the latest version. The evaluation version provides absolutely the same capabilities as the licensed version of the component. Furthermore, evaluation version simply becomes licensed when you add a few lines of code to apply the license.

### **Evaluation Version Limitations**
The evaluation version provides all the features except the following:

- **Number of Opened Files** (Aspose.Finance) When running your program, you can only open 50 files using Aspose.Finance library. If your application exceeds this number, an exception will be thrown.
- **Number of Saved Files** (Aspose.Finance) When running your program, you can only open 50 files using Aspose.Finance library. If your application exceeds this number, an exception will be thrown.

{{% alert color="primary" %}} 

If you want to try Aspose.Finance out without evaluation limitations, request a 30 day temporary license. Please refer to [How to get a Temporary License?](https://purchase.aspose.com/temporary-license) for more information.

{{% /alert %}} 
## **Applying a License**
Once you are happy with your [evaluation](https://downloads.aspose.com/finance/net) of Aspose.Finance for .NET, buy a license at the Aspose website: [Purchase Portal](https://purchase.aspose.com/buy). Make yourself familiar with the different license types available. If you have any questions, [contact the Aspose sales team](https://about.aspose.com/contact) and they'll be happy to help you.

Every Aspose license carries a one-year subscription for free upgrades to any new versions or fixes that come out during this time. We provide free and unlimited technical support to both licensed and evaluation users.

The license is a plain text XML file that contains details such as the product name, number of licensed developers, subscription expiry date and so on. The file is digitally signed, so do not modify the file: even adding an extra line break to the file invalidates it.
### **When to Apply a License**
Follow these simple rules:

- The license only needs to be set once per application domain.
- You need to set the license before using any other Aspose.Finance classes.
- Calling SetLicense multiple times is not harmful, but wastes processor time.
- If you are developing a Windows Forms or console application, call SetLicense in the startup code, before using Aspose.Finance classes.
- When developing an ASP.NET application, call SetLicense from the Global.asax.cs file, in the Aplication_Start protected method. It is called once when the application starts.
- Do not call SetLicense from within the Page_Load methods since it means the license will be loaded every time a web page is loaded.
- If you are developing a class library, you call SetLicense from a static constructor of the class that uses Aspose.Finance. The static constructor executes before an instance of your class is created making sure Aspose.Finance license is properly set.
### **Apply License using File or Stream Object**
Use the [License.SetLicense](https://apireference.aspose.com/finance/net/aspose.finance/license) method to license the component. The easiest way to set a license is to put the license file in the same folder as the Aspose.Finance.dll and specify the filename, without a path, as shown below.
#### **Loading a License from File**
This code snippet initializes a license stored in a file or in an embedded resource.

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
#### **Loading a License from a Stream Object**
These code snippets initialize the license from stream.

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
## **Apply Metered License**
Aspose.Finance for .NET API allows developers to apply metered license. It is a new licensing mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. For more details, please refer to [Metered Licensing FAQ](https://purchase.aspose.com/faqs/licensing/metered) section.

A new class [Metered](https://apireference.aspose.com/finance/net/aspose.finance/metered) has been added to apply metered key. This code example demonstrates how to set metered public and private keys:

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
