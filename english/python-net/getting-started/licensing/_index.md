---
title: Licensing
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /python-net/licensing/
description: Python Finance Library API invites its customers to get a Classic license and Metered License. As well as use a limited license to better explore the product.
---

Sometimes, in order to study the system better, you want to dive into the code as fast as possible. To make this easier, Aspose.Finance provides different plans for purchase or offers a Free Trial and a 30-day Temporary License for evaluation.

{{% alert color="primary" %}}

Note that there are a number of general policies and practices that guide you on how to evaluate, properly license, and purchase our products. You can find them in the ["Purchase Policies and FAQ"](https://purchase.aspose.com/policies) section.

{{% /alert %}}

## **Evaluate Aspose.Finance**
You can easily download Aspose.Finance for evaluation. The evaluation package is the same as the purchased package. The evaluation version simply becomes licensed after you add a few lines of code to apply the license. 

### **Evaluation Version Limitations**
The evaluation version provides all the features except the following:

- **Number of Opened Files** (Aspose.Finance) When running your program, you can only open 50 files using Aspose.Finance library. If your application exceeds this number, an exception will be thrown.
- **Number of Saved Files** (Aspose.Finance) When running your program, you can only open 50 files using Aspose.Finance library. If your application exceeds this number, an exception will be thrown.

{{% alert color="primary" %}} 

If you want to try Aspose.Finance out without evaluation limitations, request a 30 day temporary license. Please refer to [How to get a Temporary License?](https://purchase.aspose.com/temporary-license) for more information.

{{% /alert %}} 

## **About the License**
You can easily download an evaluation version of Aspose.Finance for Python via .NET from its [download page](https://pypi.org/project/aspose.finance/). The evaluation version provides absolutely **the same capabilities** as the licensed version of Aspose.Finance. Furthermore, the evaluation version simply becomes licensed after you purchase a license and add a couple of lines of code to apply the license.

The license is a plain-text XML file that contains details such as the product name, number of developers it is licensed to, subscription expiry date, and so on. The file is digitally signed, so do not modify the file. Even an inadvertent addition of an extra line break to the contents of the file will invalidate it.

To avoid the limitations associated with the evaluation version, you need to set a license before using **Aspose.Finance**. You are only required to set a license once per application or process.

## Purchased License

After purchase, you need to apply the license file or stream. This section describes options of how this can be done, and also comments on some common questions.

{{% alert color="primary" %}}

You need to set the license:
* only once per application domain
* before using any other Aspose.Finance classes

{{% /alert %}}

{{% alert color="primary" %}}

You can find pricing information on the [“Pricing Information”](https://purchase.aspose.com/pricing/finance/family) page.

{{% /alert %}}

### **Setting a License in Aspose.Finance for Python via .NET**

Licenses can be applied from various locations:

* Explicit path
* The folder containing the python script that calls Aspose.Finance for Python via .NET
* Stream
* As a Metered License – a new licensing mechanism

{{% alert color="primary" %}}

Use the **set_license** method to license a component.

Calling **set_license** multiple times is not harmful, it just wastes processor time.

{{% /alert %}}

In the sections below, we will describe the two common methods used to set the license. 

#### **Applying a License Using a File**
The easiest method of setting a license requires you to place the license file in the same folder containing the python script that calls Aspose.Finance for Python and specify just the file name without its path.

This code snippet is used to set a license file:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

When calling the set_license method, the license name should be same as that of your license file. For example, you can change the license file name to "Aspose.Finance.lic.xml". Then, in your code, you have to pass the new license name (Aspose.Finance.lic.xml) to the SetLicense method.

#### **Applying a License from a Stream**
You can load a license from a stream. 

This code snippet is used to apply a license from a stream:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Apply Metered License

Aspose.Finance allows developers to apply a metered key. This is a new licensing mechanism.

The new licensing mechanism will be used along with the existing licensing method. Those customers who want to be billed based on the use of API features can use the Metered Licensing.

After completing all the necessary steps to obtain this type of license, you will receive the keys, not the license file. This metered key can be applied using the **Metered** class specially introduced for this purpose.

The following code example shows how to set metered public and private keys:

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

Please note that you must have a stable Internet connection for the correct use of the Metered license, since the Metered mechanism requires the constant interaction with our services for correct calculations. For more details, refer to the [“Metered Licensing FAQ”](https://purchase.aspose.com/faqs/licensing/metered) section.

{{% /alert %}}
