---
title: Installation
type: docs
weight: 60
url: /fr/python-net/installation/
description: En savoir plus sur l'installation de la bibliothèque Python Finance API à l'aide de NuGet et de l'interface graphique ou de la console du gestionnaire de packages.
---
## **Configuration requise**

 Tout d'abord, vous devez vérifier et confirmer que les spécifications de la machine répondent aux[Configuration requise](/finance/fr/python-net/system-requirements/).

## **Installation de Aspose.Finance pour Python via .NET**
 `pip` est le moyen le plus simple de télécharger et d'installer[Aspose.Finance pour Python via .NET](https://pypi.org/project/aspose-finance/).

Pour installer Aspose.Finance, exécutez cette commande : pip install aspose-finance

## **Utilisation de Aspose.Finance pour Python via .NET**

Une fois que vous avez terminé l'installation du module, vous pouvez utiliser Aspose.Finance à partir de votre code python de cette façon :

```py
import aspose.finance.xbrl as afx

xbrlDoc = afx.XbrlDocument()
xbrlInstances = xbrlDoc.xbrl_instances
xbrlInstance = xbrlInstances[xbrlInstances.add()]
schemaRefs = xbrlInstance.schema_refs
schemaRefs.add(os.path.join(sourceDir, "schema.xsd"), "example", "http://example.com/xbrl/taxonomy")
xbrlDoc.save(os.path.join(outputDir, "dochavingItem.xbrl"))
```
