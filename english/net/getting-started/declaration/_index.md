---
title: Declaration
type: docs
weight: 30
url: /net/declaration/
---

## **Partial Trust / Medium Trust Challenge**
All Aspose .NET components require the Full Trust permission set. The reason is, Aspose .NET components need to access registry settings, system files other than a virtual directory for certain operations like parsing fonts, etc. Moreover, Aspose .NET Components are based on core .NET system classes that also require Full Trust permission set in many cases.

Internet Service Providers hosting multiple applications from different companies mostly enforce Medium Trust security level. In the case of .NET 2.0, such security level applies the following constraints:

- · **OleDbPermission** is not available. This means you cannot use the ADO.NET managed OLE DB data provider to access databases.
- · **EventLogPermission** is not available. This means you cannot access the Windows event log.
- · **ReflectionPermission** is not available. This means you cannot use reflection.
- · **RegistryPermission** is not available. This means you cannot access the registry.
- · **WebPermission** is restricted. This means your application can only communicate with an address or range of addresses that you define in the <trust> element.
- · **FileIOPermission** is restricted. This means you can only access files in your application's virtual directory hierarchy.

Due to the reasons specified above, Aspose .NET components cannot be used on servers granting permission set other than Full Trust.
