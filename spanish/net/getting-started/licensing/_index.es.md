---
title: Licencia
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /es/net/licensing/
description: C# Finance La Biblioteca API invita a sus clientes a obtener una licencia Clásica y una Licencia Medida. Así como utilizar una licencia limitada para explorar mejor el producto.
---
## **Evaluar Aspose.Finance**
Puede descargar fácilmente el producto Aspose.Finance for .NET con fines de evaluación. por favor refiérase a[Aspose.Finance for .NET página de descarga](https://www.nuget.org/packages/Aspose.Finance/)para conocer la última versión. La versión de evaluación proporciona absolutamente las mismas capacidades que la versión con licencia del componente. Además, la versión de evaluación simplemente obtiene la licencia cuando agrega unas pocas líneas de código para aplicar la licencia.

### **Limitaciones de la versión de evaluación**
La versión de evaluación proporciona todas las características excepto las siguientes:

- **Número de archivos abiertos** (Aspose.Finance) Al ejecutar su programa, solo puede abrir 50 archivos usando la biblioteca Aspose.Finance. Si su aplicación excede este número, se lanzará una excepción.
- **Número de archivos guardados** (Aspose.Finance) Al ejecutar su programa, solo puede abrir 50 archivos usando la biblioteca Aspose.Finance. Si su aplicación excede este número, se lanzará una excepción.

{{% alert color="primary" %}} 

 Si desea probar Aspose.Finance sin limitaciones de evaluación, solicite una licencia temporal de 30 días. Por favor refiérase a[¿Cómo obtener una Licencia Temporal?](https://purchase.aspose.com/temporary-license) para más información.

{{% /alert %}} 
## **Aplicar una licencia**
 Una vez que esté satisfecho con su[evaluación](https://downloads.aspose.com/finance/net) de Aspose.Finance for .NET, compre una licencia en el sitio web Aspose:[Portal de Compra](https://purchase.aspose.com/buy) Familiarícese con los diferentes tipos de licencia disponibles. Si tienes alguna pregunta,[póngase en contacto con el equipo de ventas Aspose](https://about.aspose.com/contact) y estarán encantados de ayudarte.

Cada licencia Aspose incluye una suscripción de un año para actualizaciones gratuitas a cualquier nueva versión o corrección que surja durante este tiempo. Brindamos soporte técnico gratuito e ilimitado a usuarios con licencia y evaluación.

La licencia es un archivo XML de texto sin formato que contiene detalles como el nombre del producto, la cantidad de desarrolladores con licencia, la fecha de vencimiento de la suscripción, etc. El archivo está firmado digitalmente, así que no lo modifique: incluso agregar un salto de línea adicional al archivo lo invalida.
### **Cuándo aplicar una licencia**
Siga estas sencillas reglas:

- La licencia solo debe establecerse una vez por dominio de aplicación.
- Debe configurar la licencia antes de usar cualquier otra clase Aspose.Finance.
- Llamar a SetLicense varias veces no es dañino, pero desperdicia tiempo de procesador.
- Si está desarrollando una aplicación de consola o formularios Windows, llame a SetLicense en el código de inicio, antes de usar las clases Aspose.Finance.
- Al desarrollar una aplicación ASP.NET, llame a SetLicense desde el archivo Global.asax.cs, en el método protegido Aplication_Start. Se llama una vez cuando se inicia la aplicación.
- No llame a SetLicense desde dentro de los métodos Page_Load, ya que significa que la licencia se cargará cada vez que se cargue una página web.
- Si está desarrollando una biblioteca de clases, llame a SetLicense desde un constructor estático de la clase que usa Aspose.Finance. El constructor estático se ejecuta antes de que se cree una instancia de su clase, asegurándose de que la licencia Aspose.Finance esté configurada correctamente.
### **Aplicar licencia usando archivo o objeto de transmisión**
 Utilizar el[Licencia.SetLicense](https://reference.aspose.com/finance/net/aspose.finance/license) para obtener la licencia del componente. La forma más fácil de configurar una licencia es colocar el archivo de licencia en la misma carpeta que Aspose.Finance.dll y especificar el nombre del archivo, sin ruta, como se muestra a continuación.
#### **Cargar una licencia desde un archivo**
Este fragmento de código inicializa una licencia almacenada en un archivo o en un recurso incrustado.

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
#### **Cargar una licencia desde un objeto de flujo**
Estos fragmentos de código inicializan la licencia de la transmisión.

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
## **Aplicar licencia medida**
Aspose.Finance for .NET API permite a los desarrolladores aplicar una licencia medida. Es un nuevo mecanismo de licencia. El nuevo mecanismo de concesión de licencias se utilizará junto con el método de concesión de licencias existente. Aquellos clientes que deseen que se les facture en función del uso de las funciones API pueden utilizar la licencia medida. Para obtener más detalles, consulte[Preguntas frecuentes sobre licencias medidas](https://purchase.aspose.com/faqs/licensing/metered)sección.

una nueva clase[medido](https://reference.aspose.com/finance/net/aspose.finance/metered)se ha agregado para aplicar la clave medida. Este ejemplo de código demuestra cómo establecer claves públicas y privadas medidas:

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
