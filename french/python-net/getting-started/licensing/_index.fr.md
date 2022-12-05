---
title: Licence
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /fr/python-net/licensing/
description: Python Finance La bibliothèque API invite ses clients à obtenir une licence classique et une licence mesurée. En plus d'utiliser une licence limitée pour mieux explorer le produit.
---
Parfois, afin de mieux étudier le système, vous souhaitez vous plonger dans le code le plus rapidement possible. Pour faciliter cela, Aspose.Finance propose différents plans d'achat ou propose un essai gratuit et une licence temporaire de 30 jours pour évaluation.

{{% alert color="primary" %}}

 Notez qu'il existe un certain nombre de politiques et de pratiques générales qui vous guident sur la façon d'évaluer, de licencier correctement et d'acheter nos produits. Vous pouvez les trouver dans le["Politiques d'achat et FAQ"](https://purchase.aspose.com/policies) section.

{{% /alert %}}

## **Évaluer Aspose.Finance**
 Vous pouvez facilement télécharger Aspose.Finance pour évaluation. Le package d'évaluation est le même que le package acheté. La version d'évaluation devient simplement sous licence après avoir ajouté quelques lignes de code pour appliquer la licence.

### **Limites de la version d'évaluation**
La version d'évaluation fournit toutes les fonctionnalités à l'exception des suivantes :

- **Nombre de fichiers ouverts** (Aspose.Finance) Lors de l'exécution de votre programme, vous ne pouvez ouvrir que 50 fichiers à l'aide de la bibliothèque Aspose.Finance. Si votre application dépasse ce nombre, une exception sera levée.
- **Nombre de fichiers enregistrés** (Aspose.Finance) Lors de l'exécution de votre programme, vous ne pouvez ouvrir que 50 fichiers à l'aide de la bibliothèque Aspose.Finance. Si votre application dépasse ce nombre, une exception sera levée.

{{% alert color="primary" %}} 

 Si vous souhaitez essayer Aspose.Finance sans limitations d'évaluation, demandez une licence temporaire de 30 jours. Prière de se référer à[Comment obtenir une licence temporaire ?](https://purchase.aspose.com/temporary-license) pour plus d'informations.

{{% /alert %}} 

## **À propos de la licence**
 Vous pouvez facilement télécharger une version d'évaluation de Aspose.Finance pour Python via .NET à partir de son[page de téléchargement](https://pypi.org/project/aspose.finance/) . La version d'évaluation fournit absolument**les mêmes capacités**en tant que version sous licence de Aspose.Finance. De plus, la version d'évaluation devient simplement sous licence après l'achat d'une licence et l'ajout de quelques lignes de code pour appliquer la licence.

La licence est un fichier XML en texte brut qui contient des détails tels que le nom du produit, le nombre de développeurs auxquels il est licencié, la date d'expiration de l'abonnement, etc. Le fichier est signé numériquement, ne modifiez donc pas le fichier. Même l'ajout par inadvertance d'un saut de ligne supplémentaire au contenu du fichier l'invalidera.

 Pour éviter les limitations associées à la version d'évaluation, vous devez définir une licence avant d'utiliser**Aspose.Finance**. Vous n'êtes tenu de définir une licence qu'une seule fois par application ou processus.

## Licence achetée

Après l'achat, vous devez appliquer le fichier de licence ou le flux. Cette section décrit les options sur la façon dont cela peut être fait, et commente également certaines questions courantes.

{{% alert color="primary" %}}

Vous devez définir la licence :
* une seule fois par domaine d'application
* avant d'utiliser toute autre classe Aspose.Finance

{{% /alert %}}

{{% alert color="primary" %}}

Vous pouvez trouver des informations sur les prix sur le["Information sur les prix"](https://purchase.aspose.com/pricing/finance/family) page.

{{% /alert %}}

### **Définition d'une licence dans Aspose.Finance pour Python via .NET**

Les licences peuvent être appliquées à partir de différents emplacements :

* Chemin explicite
* Le dossier contenant le script python qui appelle Aspose.Finance pour Python via .NET
* Flux
* En tant que licence mesurée - un nouveau mécanisme de licence

{{% alert color="primary" %}}

 Utilisez le**set_license** méthode pour licencier un composant.

 Appel**set_license** plusieurs fois n'est pas nocif, cela fait simplement perdre du temps au processeur.

{{% /alert %}}

 Dans les sections ci-dessous, nous décrirons les deux méthodes courantes utilisées pour définir la licence.

#### **Application d'une licence à l'aide d'un fichier**
La méthode la plus simple pour définir une licence nécessite de placer le fichier de licence dans le même dossier contenant le script python qui appelle Aspose.Finance pour Python et de spécifier uniquement le nom du fichier sans son chemin.

Cet extrait de code est utilisé pour définir un fichier de licence :

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

Lors de l'appel de la méthode set_license, le nom de la licence doit être le même que celui de votre fichier de licence. Par exemple, vous pouvez modifier le nom du fichier de licence en "Aspose.Finance.lic.xml". Ensuite, dans votre code, vous devez passer le nouveau nom de licence (Aspose.Finance.lic.xml) à la méthode SetLicense.

#### **Application d'une licence à partir d'un flux**
 Vous pouvez charger une licence à partir d'un flux.

Cet extrait de code est utilisé pour appliquer une licence à partir d'un flux :

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Appliquer une licence limitée

Aspose.Finance permet aux développeurs d'appliquer une clé mesurée. Il s'agit d'un nouveau mécanisme de licence.

Le nouveau mécanisme d'octroi de licences sera utilisé parallèlement à la méthode d'octroi de licences existante. Les clients qui souhaitent être facturés en fonction de l'utilisation des fonctionnalités API peuvent utiliser la licence mesurée.

 Après avoir effectué toutes les étapes nécessaires pour obtenir ce type de licence, vous recevrez les clés, et non le fichier de licence. Cette clé mesurée peut être appliquée à l'aide de la**Compteur** classe spécialement créée à cet effet.

L'exemple de code suivant montre comment définir des clés publiques et privées limitées :

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

 Veuillez noter que vous devez disposer d'une connexion Internet stable pour une utilisation correcte de la licence Metered, car le mécanisme Metered nécessite une interaction constante avec nos services pour des calculs corrects. Pour plus de détails, reportez-vous au[« FAQ sur les licences mesurées »](https://purchase.aspose.com/faqs/licensing/metered) section.

{{% /alert %}}
