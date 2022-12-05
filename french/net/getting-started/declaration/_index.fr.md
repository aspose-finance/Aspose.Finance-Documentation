---
title: Déclaration
type: docs
weight: 30
url: /fr/net/declaration/
---
## **Défi de confiance partielle/confiance moyenne**
Tous les composants Aspose .NET nécessitent l'ensemble d'autorisations Confiance totale. La raison en est que les composants Aspose .NET doivent accéder aux paramètres du registre, aux fichiers système autres qu'un répertoire virtuel pour certaines opérations telles que l'analyse des polices, etc. cas.

Les fournisseurs de services Internet hébergeant plusieurs applications de différentes sociétés appliquent principalement le niveau de sécurité Medium Trust. Dans le cas de .NET 2.0, ce niveau de sécurité applique les contraintes suivantes :

- · **OleDbPermission** n'est pas disponible. Cela signifie que vous ne pouvez pas utiliser le fournisseur de données OLE DB géré ADO.NET pour accéder aux bases de données.
- · **EventLogPermissionEventLogPermission** n'est pas disponible. Cela signifie que vous ne pouvez pas accéder au journal des événements Windows.
- · **ReflectionPermission** n'est pas disponible. Cela signifie que vous ne pouvez pas utiliser la réflexion.
- · **RegistryPermission** n'est pas disponible. Cela signifie que vous ne pouvez pas accéder au registre.
- · **WebPermission** est restreint. Cela signifie que votre application ne peut communiquer qu'avec une adresse ou une plage d'adresses que vous définissez dans le<trust> élément.
- · **FileIOPermission** est restreint. Cela signifie que vous ne pouvez accéder qu'aux fichiers de la hiérarchie de répertoires virtuels de votre application.

Pour les raisons spécifiées ci-dessus, les composants Aspose .NET ne peuvent pas être utilisés sur des serveurs accordant un ensemble d'autorisations autre que Confiance totale.
