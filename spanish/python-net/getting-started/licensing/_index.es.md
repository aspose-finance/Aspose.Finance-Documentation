---
title: Licencia
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /es/python-net/licensing/
description: Python Finance La Biblioteca API invita a sus clientes a obtener una licencia Clásica y una Licencia Medida. Así como utilizar una licencia limitada para explorar mejor el producto.
---
veces, para estudiar mejor el sistema, desea sumergirse en el código lo más rápido posible. Para hacerlo más fácil, Aspose.Finance proporciona diferentes planes de compra u ofrece una prueba gratuita y una licencia temporal de 30 días para evaluación.

{{% alert color="primary" %}}

 Tenga en cuenta que hay una serie de políticas y prácticas generales que lo guían sobre cómo evaluar, obtener la licencia adecuada y comprar nuestros productos. Puedes encontrarlos en el["Políticas de compra y preguntas frecuentes"](https://purchase.aspose.com/policies) sección.

{{% /alert %}}

## **Evaluar Aspose.Finance**
 Puede descargar fácilmente Aspose.Finance para su evaluación. El paquete de evaluación es el mismo que el paquete comprado. La versión de evaluación simplemente obtiene la licencia después de agregar algunas líneas de código para aplicar la licencia.

### **Limitaciones de la versión de evaluación**
La versión de evaluación proporciona todas las características excepto las siguientes:

- **Número de archivos abiertos** (Aspose.Finance) Al ejecutar su programa, solo puede abrir 50 archivos usando la biblioteca Aspose.Finance. Si su aplicación excede este número, se lanzará una excepción.
- **Número de archivos guardados** (Aspose.Finance) Al ejecutar su programa, solo puede abrir 50 archivos usando la biblioteca Aspose.Finance. Si su aplicación excede este número, se lanzará una excepción.

{{% alert color="primary" %}} 

 Si desea probar Aspose.Finance sin limitaciones de evaluación, solicite una licencia temporal de 30 días. Por favor refiérase a[¿Cómo obtener una Licencia Temporal?](https://purchase.aspose.com/temporary-license) para más información.

{{% /alert %}} 

## **Acerca de la licencia**
 Puede descargar fácilmente una versión de evaluación de Aspose.Finance para Python a través de .NET desde su[página de descarga](https://pypi.org/project/aspose.finance/) . La versión de evaluación proporciona absolutamente**las mismas capacidades**como la versión con licencia de Aspose.Finance. Además, la versión de evaluación simplemente obtiene la licencia después de comprar una licencia y agregar un par de líneas de código para aplicar la licencia.

La licencia es un archivo XML de texto sin formato que contiene detalles como el nombre del producto, la cantidad de desarrolladores para los que tiene licencia, la fecha de vencimiento de la suscripción, etc. El archivo está firmado digitalmente, así que no lo modifique. Incluso la adición inadvertida de un salto de línea adicional al contenido del archivo lo invalidará.

 Para evitar las limitaciones asociadas con la versión de evaluación, debe configurar una licencia antes de usar**Aspose.Finance**. Solo debe establecer una licencia una vez por aplicación o proceso.

## Licencia comprada

Después de la compra, debe aplicar el archivo de licencia o la transmisión. Esta sección describe las opciones de cómo se puede hacer esto y también comenta algunas preguntas comunes.

{{% alert color="primary" %}}

Necesita configurar la licencia:
* solo una vez por dominio de aplicación
* antes de usar cualquier otra clase Aspose.Finance

{{% /alert %}}

{{% alert color="primary" %}}

Puede encontrar información sobre precios en el["Información de precio"](https://purchase.aspose.com/pricing/finance/family) página.

{{% /alert %}}

### **Configuración de una licencia en Aspose.Finance para Python a través de .NET**

Las licencias se pueden aplicar desde varios lugares:

* Ruta explícita
* La carpeta que contiene el script de python que llama Aspose.Finance para Python a través de .NET
* Corriente
* Como licencia medida: un nuevo mecanismo de licencia

{{% alert color="primary" %}}

 Utilizar el**establecer_licencia** método para licenciar un componente.

 Vocación**establecer_licencia** varias veces no es dañino, solo desperdicia tiempo de procesador.

{{% /alert %}}

 En las siguientes secciones, describiremos los dos métodos comunes utilizados para establecer la licencia.

#### **Aplicar una licencia usando un archivo**
El método más fácil de configurar una licencia requiere que coloque el archivo de licencia en la misma carpeta que contiene el script de python que llama Aspose.Finance para Python y especifique solo el nombre del archivo sin su ruta.

Este fragmento de código se utiliza para establecer un archivo de licencia:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

Al llamar al método set_license, el nombre de la licencia debe ser el mismo que el de su archivo de licencia. Por ejemplo, puede cambiar el nombre del archivo de licencia a "Aspose.Finance.lic.xml". Luego, en su código, debe pasar el nuevo nombre de licencia (Aspose.Finance.lic.xml) al método SetLicense.

#### **Aplicación de una licencia de un flujo**
 Puede cargar una licencia desde una secuencia.

Este fragmento de código se usa para aplicar una licencia de una transmisión:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Aplicar licencia medida

Aspose.Finance permite a los desarrolladores aplicar una clave medida. Este es un nuevo mecanismo de concesión de licencias.

El nuevo mecanismo de concesión de licencias se utilizará junto con el método de concesión de licencias existente. Aquellos clientes que deseen que se les facture en función del uso de las funciones API pueden utilizar las licencias medidas.

 Después de completar todos los pasos necesarios para obtener este tipo de licencia, recibirá las claves, no el archivo de licencia. Esta clave medida se puede aplicar usando el**medido** Clase especialmente introducida para este propósito.

El siguiente ejemplo de código muestra cómo establecer claves públicas y privadas medidas:

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

 Tenga en cuenta que debe tener una conexión a Internet estable para el uso correcto de la licencia de Medida, ya que el mecanismo de Medida requiere la interacción constante con nuestros servicios para los cálculos correctos. Para obtener más detalles, consulte el["Preguntas frecuentes sobre licencias medidas"](https://purchase.aspose.com/faqs/licensing/metered) sección.

{{% /alert %}}
