---
title: Convalida i file XBRL e iXBRL in C#
linktitle: Convalida i file XBRL e iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance La biblioteca API può convalidare i file XBRL e iXBRL. Consultare i codici di esempio forniti in questo articolo per ulteriori informazioni.
type: docs
weight: 30
url: /it/net/validate-xbrl-and-ixbrl-files/
---
## **Convalidare il file di istanza XBRL in C#**
 XBRL Istanze, XBRL Linkbase e XBRL Schemi di tassonomia DEVONO rispettare i requisiti di sintassi imposti in[XBRL specifica](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Per convalidare questi, il[XbrlInstance](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) la classe fornisce il[Convalidare()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) metodo.

Il seguente frammento di codice C# illustra come convalidare un documento di istanza XBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **Convalida il file iXBRL in C#**
 Il[iXBRL specifica](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)definisce molte regole di convalida. Per la convalida dei file iXBRL, il[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) la classe fornisce a[Convalidare()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) metodo.

Il seguente frammento di codice C# illustra la convalida di un documento di istanza iXBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Codici di errore di convalida**
 Nell'enumerazione[ValidationErrorCode](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) , i codici di errore di convalida vengono definiti per ogni regola di convalida.
Di seguito sono riportate le definizioni dei codici di errore:

- ContextPeriodNoStartTime: il tipo di periodo del contesto è la durata, ma non ha una data di inizio.
- ContextPeriodNoEndTime: il tipo di periodo del contesto è la durata, ma non ha una data di fine.
- ContextPeriodStartAfterEnd: il tipo di periodo del contesto è la durata, ma la data di fine è precedente alla data di inizio.
- ContextInstantNoTime: il tipo di periodo del contesto è istantaneo, ma non ha data istantanea.
- ContextScenarioXbrlNamespace: lo scenario di contesto non può avere il nodo dello spazio dei nomi XBRL.
- ContextScenarioXbrlSubstitutionGroup: lo scenario di contesto non può avere un elemento nel gruppo di sostituzione per gli elementi definiti nello spazio dei nomi XBRL.
- ContextScenarioEmpty: lo scenario di contesto non può essere vuoto.
- ContextSegmentXbrlNamespace: il segmento di contesto non può avere il nodo dello spazio dei nomi XBRL.
- ContextSegmentXbrlSubstitutionGroup: il segmento di contesto non può avere un elemento nel gruppo di sostituzione per gli elementi definiti nello spazio dei nomi XBRL.
- ContextSegmentEmpty: il segmento di contesto non può essere vuoto.
- ItemNoContext: l'elemento deve avere un contesto.
- ItemPeroidTypeConflictWithContext: l'elemento presenta un conflitto di tipo di periodo con il contesto.
- ItemNumericNoUnit: l'elemento è numerico e deve avere un'unità.
- MonetaryItemNoSingleUnitMeasure: l'elemento è di tipo monetario e deve avere una singola unità di misura.
- MonetaryItemNoISO4217: l'articolo è di tipo monetario e deve avere un'unità di misura in stile Iso 4217.
- ShareItemNoSingleUnitMeasure: l'elemento è un tipo di condivisione e deve avere una singola unità di misura.
- ShareItemNoShareUnitMeasure: l'elemento è di tipo condiviso e deve avere un'unità di misura xbrli:shares.
- NillItemWithPrecisionOrDecimals: l'elemento è nullo e non deve avere precisione o decimali.
- FractionItemWithPrecisionOrDecimals: Item è un tipo di frazione e non deve avere precisione o decimali.
- NumericItemWithBothPrecisionAndDecimals: Item è un tipo numerico e non deve avere sia precisione che decimali.
- NumericItemWithoutPrecisionOrDecimals: Item è un tipo numerico e deve avere precisione o decimali.
- NonNumericItemWithPrecisionOrDecimals: l'elemento non è un tipo numerico e non deve avere precisione o decimali.
- FootnoteArcFromNotFound: Impossibile trovare l'arco delle note a piè di pagina da Loc.
- FootnoteArcToNotFound: impossibile trovare l'arco della nota a piè di pagina nella nota a piè di pagina.
- DefinitionArcFromNotFound: Impossibile trovare l'arco di definizione da Loc.
- DefinitionArcToNotFound: impossibile trovare l'arco di definizione in Loc.
- EssenceAliasDefinitionArcDifferentType: Essence-alias Definition arc ha diversi tipi.
- EssenceAliasDefinitionArcDifferentPeriodType: la definizione di Essence-alias arc ha diversi periodType.
- EssenceAliasDefinitionArcDifferentBalance: Essence-alias Definition arc ha diversi saldi.
- CalculationArcFromNotFound: Impossibile trovare l'arco di calcolo da Loc.
- CalculationArcToNotFound: impossibile trovare l'arco di calcolo a Loc.
- LabelArcFromNotFound: Impossibile trovare Lable arc da Loc.
- LabelArcToNotFound: Impossibile trovare l'arco Lable in Loc.
- PresentationArcFromNotFound: impossibile trovare un arco di presentazione da Loc.
- PresentationArcToNotFound: impossibile trovare un arco di presentazione in Loc.
- ReferenceArcFromNotFound: Impossibile trovare un arco di riferimento da Loc.
- ReferenceArcToNotFound: Impossibile trovare un arco di riferimento a Loc.
### **Esempio di messaggio di errore di convalida standard**
![cose da fare:immagine_alt_testo](validate-xbrl-and-ixbrl-files_1.png)

Sopra c'è un'istanza XBRL, definisce il contesto "cd1", questo tipo di periodo di contesto è la durata, la sua data di inizio è 2002-03-31, la data di fine è 2001-03-31, quindi la data di fine è precedente alla data di inizio. Nella specifica XBRL, capitolo 4.7.2, definisce la regola di convalida: "la data di fine DEVE specificare o implicare un punto nel tempo che è successivo al punto nel tempo specificato o implicito della corrispondente data di inizio". Secondo questa regola, questa istanza XBRL non è valida.
## **Convalidare XBRL e generare un messaggio di errore standard**
Il codice seguente convalida l'istanza XBRL e restituisce il messaggio di errore standard.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

L'immagine seguente mostra l'output:

![cose da fare:immagine_alt_testo](validate-xbrl-and-ixbrl-files_2.png)
## **Convalidare XBRL e generare un messaggio di errore personalizzato**
Il codice seguente convalida l'istanza XBRL e genera un messaggio di errore personalizzato.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

L'immagine seguente mostra l'output:

![cose da fare:immagine_alt_testo](validate-xbrl-and-ixbrl-files_3.png)

**Convalidare XBRL e generare un messaggio di errore standard**


