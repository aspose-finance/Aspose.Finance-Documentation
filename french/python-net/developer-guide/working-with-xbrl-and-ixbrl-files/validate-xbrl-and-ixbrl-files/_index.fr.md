---
title: Valider les fichiers XBRL et iXBRL en Python
linktitle: Valider les fichiers XBRL et iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance La bibliothèque API peut valider les fichiers XBRL et iXBRL. Veuillez consulter les exemples de codes donnés dans cet article pour plus d'informations.
type: docs
weight: 30
url: /fr/python-net/validate-xbrl-and-ixbrl-files/
---
## **Valider le fichier d'instance XBRL dans Python**
 Les instances XBRL, les bases de liens XBRL et les schémas de taxonomie XBRL DOIVENT être conformes aux exigences de syntaxe imposées dans[Spécification XBRL](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Pour les valider, la classe XbrlInstance fournit la méthode validate().

L'extrait de code Python suivant montre comment valider un document d'instance XBRL.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **Valider le dossier iXBRL en Python**
 La[Spécification iXBRL](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html) définit de nombreuses règles de validation. Pour valider les fichiers iXBRL, la classe InlineXbrlDocument fournit une méthode validate().

L'extrait de code Python suivant illustre la validation d'un document d'instance iXBRL.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **Codes d'erreur de validation**
 Dans l'énumération ValidationErrorCode, les codes d'erreur de validation sont définis pour chaque règle de validation.
Voici les définitions des codes d'erreur :

- LE CONTEXTE_PÉRIODE_NON_DÉBUT_TIME : le type de période de contexte est une durée, mais n'a pas de date de début.
- LE CONTEXTE_PÉRIODE_NON_FIN_TIME : le type de période de contexte est une durée, mais n'a pas de date de fin.
- LE CONTEXTE_PÉRIODE_DÉBUT_APRÈS_FIN : le type de période de contexte est la durée, mais la date de fin est antérieure à la date de début.
- LE CONTEXTE_INSTANTANÉ_NO_TIME : le type de période de contexte est instantané, mais n'a pas de date instantanée.
- LE CONTEXTE_SCÉNARIO_XBRL_NAMESPACE : le scénario de contexte ne peut pas avoir de nœud d'espace de noms XBRL.
- LE CONTEXTE_SCÉNARIO_XBRL_SUBSTITUTION_GROUP : Le scénario de contexte ne peut pas avoir d'élément dans le groupe de substitution pour les éléments définis dans l'espace de noms XBRL.
- LE CONTEXTE_SCÉNARIO_VIDE : le scénario de contexte ne peut pas être vide.
- LE CONTEXTE_SEGMENT_XBRL_NAMESPACE : le segment de contexte ne peut pas avoir le nœud d'espace de noms XBRL.
- LE CONTEXTE_SEGMENT_XBRL_SUBSTITUTIONGROUP : le segment de contexte ne peut pas avoir d'élément dans le groupe de substitution pour les éléments définis dans l'espace de noms XBRL.
- LE CONTEXTE_SEGMENT_VIDE : le segment de contexte ne peut pas être vide.
- OBJET_NON_CONTEXTE : l'élément doit avoir un contexte.
- OBJET_PÉRIODE_TAPER_CONFLIT_WITH_CONTEXT : l'élément a un conflit de type de période avec le contexte.
- OBJET_NUMÉRIQUE_NO_UNIT : l'élément est numérique et doit avoir une unité.
- MONÉTAIRE_OBJET_NON_CÉLIBATAIRE_UNIT_MEASURE : l'élément est un type monétaire et doit avoir une seule unité de mesure.
- MONÉTAIRE_OBJET_NO_ISO4217 : l'article est un type monétaire et doit avoir une unité de mesure de style ISO 4217.
- PARTAGER_OBJET_NON_CÉLIBATAIRE_UNIT_MEASURE : l'élément est un type de partage et doit avoir une seule unité de mesure.
- PARTAGER_OBJET_NON_PARTAGER_UNIT_MEASURE : l'élément est de type partage et doit avoir une unité de mesure xbrli:shares.
- NUL_OBJET_AVEC_PRÉCISION_OR_DECIMALS : l'élément est nil et ne doit avoir ni précision ni décimales.
- FRACTION_OBJET_AVEC_PRÉCISION_OR_DECIMALS : l'élément est un type de fraction et ne doit pas avoir de précision ni de décimales.
- NUMÉRIQUE_OBJET_AVEC_TOUS LES DEUX_PRÉCISION_ET_DECIMALS : l'élément est un type numérique et ne doit pas avoir à la fois une précision et des décimales.
- NUMÉRIQUE_OBJET_SANS POUR AUTANT_PRÉCISION_OR_DECIMALS : l'élément est un type numérique et doit avoir une précision ou des décimales.
- NON_NUMÉRIQUE_OBJET_AVEC_PRÉCISION_OU_DECIMALS : l'élément n'est pas un type numérique et ne doit pas avoir de précision ni de décimales.
- NOTE DE BAS DE PAGE_ARC_DE_NE PAS_TROUVÉ : Impossible de trouver l'arc de note de bas de page à partir de Loc.
- NOTE DE BAS DE PAGE_ARC_À_NE PAS_TROUVÉ : impossible de trouver l'arc de la note de bas de page vers la note de bas de page.
- DÉFINITION_ARC_DE_NE PAS_TROUVÉ : Impossible de trouver l'arc de définition à partir de Loc.
- DÉFINITION_ARC_À_NE PAS_TROUVÉ : Impossible de trouver l'arc de définition vers Loc.
- ESSENCE_ALIAS_DÉFINITION_ARC_DIFFERENT_TYPE : l'arc de définition Essence-alias a différents types.
- ESSENCE_ALIAS_DÉFINITION_ARC_DIFFÉRENT_PÉRIODE_TYPE : l'arc de définition d'alias d'essence a différents periodTypes.
- ESSENCE_ALIAS_DÉFINITION_ARC_DIFFERENT_BALANCE : l'arc de définition d'essence-alias a des soldes différents.
- CALCUL_ARC_DE_NE PAS_TROUVÉ : Impossible de trouver l'arc de calcul à partir de Loc.
- CALCUL_ARC_À_NE PAS_TROUVÉ : Impossible de trouver l'arc de calcul vers Loc.
- ÉTIQUETTE_ARC_DE_NE PAS_TROUVÉ : Impossible de trouver l'arc Lable de Loc.
- ÉTIQUETTE_ARC_À_NE PAS_TROUVÉ : Impossible de trouver l'arc de l'étiquette vers Loc.
- PRÉSENTATION_ARC_DE_NE PAS_TROUVÉ : Impossible de trouver un arc de présentation à partir de Loc.
- PRÉSENTATION_ARC_À_NE PAS_TROUVÉ : Impossible de trouver un arc de présentation à Loc.
- RÉFÉRENCE_ARC_DE_NE PAS_TROUVÉ : Impossible de trouver un arc de référence à partir de Loc.
- RÉFÉRENCE_ARC_À_NE PAS_TROUVÉ : Impossible de trouver un arc de référence à Loc.
### **Exemple de message d'erreur de validation standard**
![tâche : image_autre_texte](validate-xbrl-and-ixbrl-files_1.png)

Ci-dessus est une instance XBRL, elle définit le contexte "cd1", ce type de période de contexte est la durée, sa date de début est le 2002-03-31, la date de fin est le 2001-03-31, donc la date de fin est antérieure à la date de début. Dans la spécification XBRL, chapitre 4.7.2, elle définit la règle de validation : "la date de fin DOIT spécifier ou impliquer un point dans le temps postérieur au point dans le temps spécifié ou implicite de la date de début correspondante". Selon cette règle, cette instance XBRL n'est pas valide.
## **Validez XBRL et affichez le message d'erreur standard**
Le code suivant valide l'instance XBRL et génère le message d'erreur standard.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

L'image suivante montre la sortie :

![tâche : image_autre_texte](validate-xbrl-and-ixbrl-files_2.png)



