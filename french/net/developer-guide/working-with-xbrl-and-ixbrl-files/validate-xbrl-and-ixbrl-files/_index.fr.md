---
title: Valider les fichiers XBRL et iXBRL en C#
linktitle: Valider les fichiers XBRL et iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance La bibliothèque API peut valider les fichiers XBRL et iXBRL. Veuillez consulter les exemples de codes donnés dans cet article pour plus d'informations.
type: docs
weight: 30
url: /fr/net/validate-xbrl-and-ixbrl-files/
---
## **Valider le fichier d'instance XBRL dans C#**
 Les instances XBRL, les bases de liens XBRL et les schémas de taxonomie XBRL DOIVENT être conformes aux exigences de syntaxe imposées dans[Spécification XBRL](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Pour les valider, le[XbrlInstance](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) la classe fournit la[Valider()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) méthode.

L'extrait de code C# suivant montre comment valider un document d'instance XBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **Valider le dossier iXBRL en C#**
 La[Spécification iXBRL](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)définit de nombreuses règles de validation. Pour valider les fichiers iXBRL, le[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) la classe offre une[Valider()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) méthode.

L'extrait de code C# suivant illustre la validation d'un document d'instance iXBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Codes d'erreur de validation**
 Dans l'énumération[CodeErreurValidation](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) , des codes d'erreur de validation sont définis pour chaque règle de validation.
Voici les définitions des codes d'erreur :

- ContextPeriodNoStartTime : le type de période de contexte est une durée, mais n'a pas de date de début.
- ContextPeriodNoEndTime : le type de période de contexte est une durée, mais n'a pas de date de fin.
- ContextPeriodStartAfterEnd : le type de période de contexte est la durée, mais la date de fin est antérieure à la date de début.
- ContextInstantNoTime : le type de période de contexte est instantané, mais n'a pas de date instantanée.
- ContextScenarioXbrlNamespace : le scénario de contexte ne peut pas avoir de nœud d'espace de noms XBRL.
- ContextScenarioXbrlSubstitutionGroup : le scénario de contexte ne peut pas avoir d'élément dans le groupe de substitution pour les éléments définis dans l'espace de noms XBRL.
- ContextScenarioEmpty : le scénario de contexte ne peut pas être vide.
- ContextSegmentXbrlNamespace : le segment de contexte ne peut pas avoir le nœud d'espace de noms XBRL.
- ContextSegmentXbrlSubstitutionGroup : le segment de contexte ne peut pas avoir d'élément dans le groupe de substitution pour les éléments définis dans l'espace de noms XBRL.
- ContextSegmentEmpty : le segment de contexte ne peut pas être vide.
- ItemNoContext : l'élément doit avoir un contexte.
- ItemPeroidTypeConflictWithContext : l'élément a un conflit de type de période avec le contexte.
- ItemNumericNoUnit : l'élément est numérique et doit avoir une unité.
- MonetaryItemNoSingleUnitMeasure : Item est un type monétaire et doit avoir une seule unité de mesure.
- MonetaryItemNoISO4217 : l'élément est un type monétaire et doit avoir une unité de mesure de style Iso 4217.
- ShareItemNoSingleUnitMeasure : l'élément est un type de partage et doit avoir une seule unité de mesure.
- ShareItemNoShareUnitMeasure : l'élément est de type partage et doit avoir une unité de mesure xbrli:shares.
- NillItemWithPrecisionOrDecimals : l'élément est nil et ne doit avoir ni précision ni décimales.
- FractionItemWithPrecisionOrDecimals : l'élément est un type de fraction et ne doit pas avoir de précision ni de décimales.
- NumericItemWithBothPrecisionAndDecimals : Item est un type numérique et ne doit pas avoir à la fois précision et décimales.
- NumericItemWithoutPrecisionOrDecimals : Item est un type numérique et doit avoir une précision ou des décimales.
- NonNumericItemWithPrecisionOrDecimals : Item n'est pas un type numérique et ne doit pas avoir de précision ni de décimales.
- FootnoteArcFromNotFound : impossible de trouver l'arc de note de bas de page à partir de Loc.
- FootnoteArcToNotFound : impossible de trouver l'arc de la note de bas de page vers la note de bas de page.
- DefinitionArcFromNotFound : impossible de trouver l'arc de définition à partir de Loc.
- DefinitionArcToNotFound : impossible de trouver l'arc de définition vers Loc.
- EssenceAliasDefinitionArcDifferentType : l'arc de définition d'alias d'essence a différents types.
- EssenceAliasDefinitionArcDifferentPeriodType : l'arc de définition d'alias d'essence a différents periodTypes.
- EssenceAliasDefinitionArcDifferentBalance : l'arc de définition d'alias d'essence a des soldes différents.
- CalculationArcFromNotFound : impossible de trouver l'arc de calcul à partir de Loc.
- CalculationArcToNotFound : impossible de trouver l'arc de calcul vers Loc.
- LabelArcFromNotFound : impossible de trouver l'arc Lable à partir de Loc.
- LabelArcToNotFound : impossible de trouver l'arc Lable vers Loc.
- PresentationArcFromNotFound : impossible de trouver un arc de présentation à partir de Loc.
- PresentationArcToNotFound : impossible de trouver un arc de présentation à Loc.
- ReferenceArcFromNotFound : impossible de trouver un arc de référence à partir de Loc.
- ReferenceArcToNotFound : impossible de trouver un arc de référence à Loc.
### **Exemple de message d'erreur de validation standard**
![tâche : image_autre_texte](validate-xbrl-and-ixbrl-files_1.png)

Ci-dessus est une instance XBRL, elle définit le contexte "cd1", ce type de période de contexte est la durée, sa date de début est le 2002-03-31, la date de fin est le 2001-03-31, donc la date de fin est antérieure à la date de début. Dans la spécification XBRL, chapitre 4.7.2, elle définit la règle de validation : "la date de fin DOIT spécifier ou impliquer un point dans le temps postérieur au point dans le temps spécifié ou implicite de la date de début correspondante". Selon cette règle, cette instance XBRL n'est pas valide.
## **Validez XBRL et affichez le message d'erreur standard**
Le code suivant valide l'instance XBRL et génère le message d'erreur standard.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

L'image suivante montre la sortie :

![tâche : image_autre_texte](validate-xbrl-and-ixbrl-files_2.png)
## **Validez XBRL et affichez un message d'erreur personnalisé**
Le code suivant valide l'instance XBRL et génère un message d'erreur personnalisé.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

L'image suivante montre la sortie :

![tâche : image_autre_texte](validate-xbrl-and-ixbrl-files_3.png)

**Validez XBRL et affichez le message d'erreur standard**


