---
title: Licence
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /fr/net/licensing/
description: C# Finance La bibliothèque API invite ses clients à obtenir une licence classique et une licence mesurée. En plus d'utiliser une licence limitée pour mieux explorer le produit.
---
## **Évaluer Aspose.Finance**
Vous pouvez facilement télécharger le produit Aspose.Finance for .NET à des fins d'évaluation. Veuillez vous référer au[Aspose.Finance for .NET page de téléchargement](https://www.nuget.org/packages/Aspose.Finance/)pour connaître la dernière version. La version d'évaluation fournit absolument les mêmes fonctionnalités que la version sous licence du composant. De plus, la version d'évaluation devient simplement sous licence lorsque vous ajoutez quelques lignes de code pour appliquer la licence.

### **Limites de la version d'évaluation**
La version d'évaluation fournit toutes les fonctionnalités à l'exception des suivantes :

- **Nombre de fichiers ouverts** (Aspose.Finance) Lors de l'exécution de votre programme, vous ne pouvez ouvrir que 50 fichiers à l'aide de la bibliothèque Aspose.Finance. Si votre application dépasse ce nombre, une exception sera levée.
- **Nombre de fichiers enregistrés** (Aspose.Finance) Lors de l'exécution de votre programme, vous ne pouvez ouvrir que 50 fichiers à l'aide de la bibliothèque Aspose.Finance. Si votre application dépasse ce nombre, une exception sera levée.

{{% alert color="primary" %}} 

 Si vous souhaitez essayer Aspose.Finance sans limitations d'évaluation, demandez une licence temporaire de 30 jours. Prière de se référer à[Comment obtenir une licence temporaire ?](https://purchase.aspose.com/temporary-license) pour plus d'informations.

{{% /alert %}} 
## **Appliquer une licence**
 Une fois que vous êtes satisfait de votre[évaluation](https://downloads.aspose.com/finance/net) du Aspose.Finance for .NET, achetez une licence sur le site Aspose :[Portail d'achat](https://purchase.aspose.com/buy) Familiarisez-vous avec les différents types de licences disponibles. Si vous avez des questions,[contacter l'équipe commerciale Aspose](https://about.aspose.com/contact) et ils seront heureux de vous aider.

Chaque licence Aspose comporte un abonnement d'un an pour des mises à niveau gratuites vers toutes les nouvelles versions ou correctifs qui sortent pendant cette période. Nous fournissons un support technique gratuit et illimité aux utilisateurs sous licence et d'évaluation.

La licence est un fichier XML en texte brut qui contient des détails tels que le nom du produit, le nombre de développeurs sous licence, la date d'expiration de l'abonnement, etc. Le fichier est signé numériquement, ne modifiez donc pas le fichier : même l'ajout d'un saut de ligne supplémentaire au fichier l'invalide.
### **Quand appliquer une licence**
Suivez ces règles simples :

- La licence ne doit être définie qu'une seule fois par domaine d'application.
- Vous devez définir la licence avant d'utiliser toute autre classe Aspose.Finance.
- Appeler SetLicense plusieurs fois n'est pas dangereux, mais fait perdre du temps au processeur.
- Si vous développez une application Windows Forms ou console, appelez SetLicense dans le code de démarrage avant d'utiliser les classes Aspose.Finance.
- Lors du développement d'une application ASP.NET, appelez SetLicense à partir du fichier Global.asax.cs, dans la méthode protégée Aplication_Start. Il est appelé une fois au démarrage de l'application.
- N'appelez pas SetLicense à partir des méthodes Page_Load car cela signifie que la licence sera chargée à chaque chargement d'une page Web.
- Si vous développez une bibliothèque de classes, vous appelez SetLicense à partir d'un constructeur statique de la classe qui utilise Aspose.Finance. Le constructeur statique s'exécute avant qu'une instance de votre classe soit créée en s'assurant que la licence Aspose.Finance est correctement définie.
### **Appliquer la licence à l'aide d'un fichier ou d'un objet de flux**
 Utilisez le[Licence.SetLicense](https://reference.aspose.com/finance/net/aspose.finance/license) méthode pour obtenir la licence du composant. Le moyen le plus simple de définir une licence consiste à placer le fichier de licence dans le même dossier que Aspose.Finance.dll et à spécifier le nom du fichier, sans chemin, comme indiqué ci-dessous.
#### **Chargement d'une licence à partir d'un fichier**
Cet extrait de code initialise une licence stockée dans un fichier ou dans une ressource intégrée.

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
#### **Chargement d'une licence à partir d'un objet de flux**
Ces extraits de code initialisent la licence à partir du flux.

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
## **Appliquer une licence limitée**
Aspose.Finance for .NET API permet aux développeurs d'appliquer une licence limitée. Il s'agit d'un nouveau mécanisme d'octroi de licences. Le nouveau mécanisme d'octroi de licences sera utilisé avec la méthode d'octroi de licences existante. Les clients qui souhaitent être facturés en fonction de l'utilisation des fonctionnalités API peuvent utiliser la licence mesurée. Pour plus de détails, veuillez consulter[FAQ sur les licences limitées](https://purchase.aspose.com/faqs/licensing/metered)section.

Une nouvelle classe[Compteur](https://reference.aspose.com/finance/net/aspose.finance/metered)a été ajouté pour appliquer la clé mesurée. Cet exemple de code montre comment définir des clés publiques et privées limitées :

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
