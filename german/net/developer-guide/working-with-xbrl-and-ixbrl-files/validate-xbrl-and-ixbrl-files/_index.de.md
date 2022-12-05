---
title: Validieren Sie die Dateien XBRL und iXBRL in C#
linktitle: Validieren Sie die Dateien XBRL und iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance Bibliothek API kann XBRL- und iXBRL-Dateien validieren. Weitere Informationen finden Sie in den Beispielcodes in diesem Artikel.
type: docs
weight: 30
url: /de/net/validate-xbrl-and-ixbrl-files/
---
## **Validieren Sie die Instanzdatei XBRL in C#**
 XBRL-Instanzen, XBRL-Linkbases und XBRL-Taxonomieschemata MÜSSEN den in[XBRL Spezifikation](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Um diese zu validieren, die[XbrlInstance](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) Klasse bietet die[Bestätigen()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) Methode.

Das folgende C#-Code-Snippet zeigt, wie ein XBRL-Instanzdokument validiert wird.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **Validieren Sie die iXBRL-Datei in C#**
 Das[iXBRL Spezifikation](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)definiert viele Validierungsregeln. Für die Validierung von iXBRL-Dateien ist die[InlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) Klasse bietet a[Bestätigen()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) Methode.

Das folgende C#-Code-Snippet veranschaulicht die Validierung eines iXBRL-Instanzdokuments.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Validierungsfehlercodes**
 In der Aufzählung[Validierungsfehlercode](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) werden Validierungsfehlercodes für jede Validierungsregel definiert.
Im Folgenden sind die Definitionen der Fehlercodes aufgeführt:

- ContextPeriodNoStartTime: Der Typ des Kontextzeitraums ist Dauer, hat aber kein Startdatum.
- ContextPeriodNoEndTime: Der Kontextzeitraumtyp ist Dauer, hat aber kein Enddatum.
- ContextPeriodStartAfterEnd: Der Typ des Kontextzeitraums ist Dauer, aber das Enddatum liegt vor dem Startdatum.
- ContextInstantNoTime: Der Kontextzeitraumtyp ist Instant, hat aber kein Instant-Datum.
- ContextScenarioXbrlNamespace: Das Kontextszenario darf keinen XBRL-Namespace-Knoten haben.
- ContextScenarioXbrlSubstitutionGroup: Das Kontextszenario darf kein Element in der Substitutionsgruppe für Elemente haben, die im Namensraum XBRL definiert sind.
- ContextScenarioEmpty: Kontextszenario darf nicht leer sein.
- ContextSegmentXbrlNamespace: Das Kontextsegment darf keinen XBRL-Namespace-Knoten haben.
- ContextSegmentXbrlSubstitutionGroup: Das Kontextsegment darf kein Element in der Substitutionsgruppe für Elemente haben, die im Namensraum XBRL definiert sind.
- ContextSegmentEmpty: Kontextsegment darf nicht leer sein.
- ItemNoContext: Item muss einen Kontext haben.
- ItemPeroidTypeConflictWithContext: Artikel hat Zeitraumtypkonflikt mit Kontext.
- ItemNumericNoUnit: Item ist numerisch und muss eine Einheit haben.
- MonetaryItemNoSingleUnitMeasure: Artikel ist ein Geldtyp und muss eine einzelne Maßeinheit haben.
- MonetaryItemNoISO4217: Der Artikel ist ein Geldtyp und muss eine Maßeinheit im Stil von Iso 4217 haben.
- ShareItemNoSingleUnitMeasure: Artikel ist ein Anteilstyp und muss eine einzelne Maßeinheit haben.
- ShareItemNoShareUnitMeasure: Das Element ist vom Typ „Share“ und muss eine xbrli:shares-Maßeinheit haben.
- NillItemWithPrecisionOrDecimals: Das Element ist null und darf weder Genauigkeit noch Dezimalstellen haben.
- FractionItemWithPrecisionOrDecimals: Item ist ein Bruchtyp und darf weder Genauigkeit noch Dezimalstellen haben.
- NumericItemWithBothPrecisionAndDecimals: Item ist ein numerischer Typ und darf nicht sowohl Genauigkeit als auch Dezimalstellen aufweisen.
- NumericItemWithoutPrecisionOrDecimals: Item ist ein numerischer Typ und muss entweder Genauigkeit oder Dezimalstellen aufweisen.
- NonNumericItemWithPrecisionOrDecimals: Item ist kein numerischer Typ und darf weder Genauigkeit noch Dezimalstellen haben.
- FootnoteArcFromNotFound: Fußnotenbogen von Loc kann nicht gefunden werden.
- FootnoteArcToNotFound: Bogen von Fußnote zu Fußnote kann nicht gefunden werden.
- DefinitionArcFromNotFound: Definitionsbogen von Loc kann nicht gefunden werden.
- DefinitionArcToNotFound: Definitionsbogen zu Loc kann nicht gefunden werden.
- EssenceAliasDefinitionArcDifferentType: Essence-Alias-Definitionsbogen hat verschiedene Typen.
- EssenceAliasDefinitionArcDifferentPeriodType: Essence-Alias Definition arc hat verschiedene periodTypes.
- EssenceAliasDefinitionArcDifferentBalance: Essence-Alias Definition arc hat unterschiedliche Balancen.
- CalculationArcFromNotFound: Berechnungsbogen von Loc kann nicht gefunden werden.
- CalculationArcToNotFound: Berechnungsbogen zu Loc kann nicht gefunden werden.
- LabelArcFromNotFound: Beschriftungsbogen von Loc kann nicht gefunden werden.
- LabelArcToNotFound: Lable-Bogen zu Loc kann nicht gefunden werden.
- PresentationArcFromNotFound: Es konnte kein Präsentationsbogen von Loc gefunden werden.
- PresentationArcToNotFound: Präsentationsbogen zu Loc konnte nicht gefunden werden.
- ReferenceArcFromNotFound: Referenzbogen von Loc kann nicht gefunden werden.
- ReferenceArcToNotFound: Referenzbogen zu Loc kann nicht gefunden werden.
### **Beispiel für eine standardmäßige Validierungsfehlermeldung**
![todo: Bild_alt_Text](validate-xbrl-and-ixbrl-files_1.png)

Oben ist eine XBRL-Instanz, sie definiert den Kontext „cd1“, dieser Kontextzeitraumtyp ist Dauer, sein Startdatum ist 2002-03-31, das Enddatum ist 2001-03-31, also liegt das Enddatum vor dem Startdatum. In der XBRL-Spezifikation, Kapitel 4.7.2, definiert sie eine Validierungsregel: „das Enddatum MUSS einen Zeitpunkt spezifizieren oder implizieren, der nach dem angegebenen oder implizierten Zeitpunkt des entsprechenden Startdatums liegt“. Gemäß dieser Regel ist diese XBRL-Instanz nicht gültig.
## **XBRL validieren und Standardfehlermeldung ausgeben**
Der folgende Code validiert die Instanz XBRL und gibt die Standardfehlermeldung aus.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

Das folgende Bild zeigt die Ausgabe:

![todo: Bild_alt_Text](validate-xbrl-and-ixbrl-files_2.png)
## **Validieren Sie XBRL und geben Sie eine angepasste Fehlermeldung aus**
Der folgende Code validiert die Instanz XBRL und gibt eine benutzerdefinierte Fehlermeldung aus.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

Das folgende Bild zeigt die Ausgabe:

![todo: Bild_alt_Text](validate-xbrl-and-ixbrl-files_3.png)

**XBRL validieren und Standardfehlermeldung ausgeben**


