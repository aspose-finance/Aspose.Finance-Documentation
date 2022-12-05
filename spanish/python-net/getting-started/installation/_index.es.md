---
title: Instalación
type: docs
weight: 60
url: /es/python-net/installation/
description: Obtenga información sobre la instalación de la biblioteca Python Finance API mediante NuGet y la GUI o la consola del administrador de paquetes.
---
## **Requisitos del sistema**

 Primero, debe verificar y confirmar que las especificaciones de la máquina cumplen con los[Requisitos del sistema](/finance/es/python-net/system-requirements/).

## **Instalación de Aspose.Finance para Python a través de .NET**
 `pip` es la forma más fácil de descargar e instalar[Aspose.Finance para Python vía .NET](https://pypi.org/project/aspose-finance/).

Para instalar Aspose.Finance, ejecute este comando: pip install aspose-finance

## **Usando Aspose.Finance para Python vía .NET**

Una vez que termine de instalar el módulo, puede usar Aspose.Finance desde su código python de esta manera:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
