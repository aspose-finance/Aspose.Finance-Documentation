---
title: Installazione
type: docs
weight: 60
url: /it/python-net/installation/
description: Informazioni sull'installazione della libreria Python Finance API utilizzando NuGet e la GUI o la console di Package Manager.
---
## **Requisiti di sistema**

 In primo luogo, è necessario verificare e confermare che le specifiche della macchina soddisfino i requisiti[requisiti di sistema](/finance/it/python-net/system-requirements/).

## **Installazione di Aspose.Finance per Python tramite .NET**
 `pip` è il modo più semplice per scaricare e installare[Aspose.Finance per Python tramite .NET](https://pypi.org/project/aspose-finance/).

Per installare Aspose.Finance, eseguire questo comando: pip install aspose-finance

## **Utilizzando Aspose.Finance per Python tramite .NET**

Una volta terminata l'installazione del modulo, puoi utilizzare Aspose.Finance dal tuo codice Python in questo modo:

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
