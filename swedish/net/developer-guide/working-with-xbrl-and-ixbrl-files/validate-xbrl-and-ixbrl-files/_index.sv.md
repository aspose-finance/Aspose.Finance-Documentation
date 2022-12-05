---
title: Validera filerna XBRL och iXBRL i C#
linktitle: Validera filerna XBRL och iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance Bibliotek API kan validera XBRL och iXBRL filer. Se exempelkoderna i den här artikeln för mer information.
type: docs
weight: 30
url: /sv/net/validate-xbrl-and-ixbrl-files/
---
## **Validera instansfilen XBRL i C#**
 XBRL Instances, XBRL Linkbases och XBRL Taxonomy Schemas MÅSTE uppfylla syntaxkraven i[XBRL specifikation](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). För att validera dessa,[XbrlInstance](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) klass ger[Bekräfta()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) metod.

Följande C#-kodavsnitt visar hur man validerar ett XBRL-instansdokument.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **Validera filen iXBRL i C#**
 De[iXBRL specifikation](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)definierar många valideringsregler. För att validera iXBRL-filer,[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) klass ger en[Bekräfta()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) metod.

Följande C#-kodavsnitt visar validering av ett iXBRL-instansdokument.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Validering felkoder**
 I uppräkningen[ValidationErrorCode](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) , valideringsfelkoder definieras för varje valideringsregel.
Följande är felkodsdefinitionerna:

- ContextPeriodNoStartTime: Typ av kontextperiod är varaktighet, men har inget startdatum.
- ContextPeriodNoEndTime: Typ av kontextperiod är varaktighet, men har inget slutdatum.
- ContextPeriodStartAfterEnd: Typ av kontextperiod är varaktighet, men slutdatumet är före startdatumet.
- ContextInstantNoTime: Kontextperiodtypen är omedelbar, men har inget direktdatum.
- ContextScenarioXbrlNamespace: Kontextscenariot kan inte ha XBRL namnområdesnod.
- ContextScenarioXbrlSubstitutionGroup: Kontextscenariot kan inte ha ett element i ersättningsgruppen för element definierade i namnområdet XBRL.
- ContextScenarioEmpty: Kontextscenariot kan inte vara tomt.
- ContextSegmentXbrlNamespace: Kontextsegment kan inte ha XBRL namnområdesnod.
- ContextSegmentXbrlSubstitutionGroup: Kontextsegmentet kan inte ha element i substitutionsgruppen för element definierade i namnrymden XBRL.
- ContextSegmentEmpty: Kontextsegmentet får inte vara tomt.
- ItemNoContext: Objekt måste ha ett sammanhang.
- ItemPeroidTypeConflictWithContext: Objektet har periodtypkonflikt med sammanhanget.
- ItemNumericNoUnit: Objektet är numeriskt och måste ha en enhet.
- MonetaryItemNoSingleUnitMeasure: Objektet är en monetär typ och måste ha ett enda mått.
- MonetaryItemNoISO4217: Artikeln är en monetär typ och måste ha en Iso 4217 stil enhetsmått.
- ShareItemNoSingleUnitMeasure: Objektet är en delningstyp och måste ha ett enda mått.
- ShareItemNoShareUnitMeasure: Objektet är delningstyp och måste ha ett xbrli:shares enhetsmått.
- NillItemWithPrecisionOrDecimals: Artikeln är noll och får inte ha vare sig precision eller decimaler.
- FractionItemWithPrecisionOrDecimals: Objektet är en bråktyp och får inte ha vare sig precision eller decimaler.
- NumericItemWithBothPrecisionAndDecimals: Objektet är en numerisk typ och får inte ha både precision och decimaler.
- NumericItemWithoutPrecisionOrDecimals: Objektet är en numerisk typ och måste ha antingen precision eller decimaler.
- NonNumericItemWithPrecisionOrDecimals: Objektet är inte en numerisk typ och får inte ha vare sig precision eller decimaler.
- FootnoteArcFromNotFound: Det gick inte att hitta fotnotsbågen från Loc.
- FootnoteArcToNotFound: Det gick inte att hitta fotnotsbåge till fotnot.
- DefinitionArcFromNotFound: Det gick inte att hitta definitionsbågen från Loc.
- DefinitionArcToNotFound: Det gick inte att hitta definitionsbågen till Loc.
- EssenceAliasDefinitionArcDifferentType: Essence-alias Definition arc har olika typer.
- EssenceAliasDefinitionArcDifferentPeriodType: Essence-alias Definition arc har olika periodTypes.
- EssenceAliasDefinitionArcDifferentBalance: Essence-alias Definition arc har olika balanser.
- CalculationArcFromNotFound: Kan inte hitta beräkningsbåge från Loc.
- CalculationArcToNotFound: Det gick inte att hitta beräkningsbågen till Loc.
- LabelArcFromNotFound: Kan inte hitta etikettbågen från Loc.
- LabelArcToNotFound: Kan inte hitta etikettbågen till Loc.
- PresentationArcFromNotFound: Det gick inte att hitta en presentationsbåge från Loc.
- PresentationArcToNotFound: Det gick inte att hitta en presentationsbåge till Loc.
- ReferenceArcFromNotFound: Det gick inte att hitta en referensbåge från Loc.
- ReferenceArcToNotFound: Det gick inte att hitta en referensbåge till Loc.
### **Exempel på standard valideringsfelmeddelande**
![todo:image_alt_text](validate-xbrl-and-ixbrl-files_1.png)

Ovan är en XBRL-instans, den definierar sammanhanget "cd1", denna kontextperiodtyp är varaktighet, dess startdatum är 2002-03-31, slutdatumet är 2001-03-31, så slutdatumet är före startdatumet. I XBRL-specifikationen, kapitel 4.7.2, definierar den valideringsregeln: "slutdatumet MÅSTE ange eller antyda en tidpunkt som är senare än den angivna eller underförstådda tidpunkten för motsvarande startdatum". Enligt denna regel är denna XBRL-instans inte en giltig.
## **Validera XBRL och mata ut standardfelmeddelande**
Följande kod validerar XBRL-instansen och matar ut standardfelmeddelandet.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

Följande bild visar resultatet:

![todo:image_alt_text](validate-xbrl-and-ixbrl-files_2.png)
## **Validera XBRL och mata ut anpassat felmeddelande**
Följande kod validerar XBRL-instansen och skickar ut anpassat felmeddelande.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

Följande bild visar resultatet:

![todo:image_alt_text](validate-xbrl-and-ixbrl-files_3.png)

**Validera XBRL och mata ut standardfelmeddelande**


