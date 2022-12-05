---
title: Validieren Sie die Dateien XBRL und iXBRL in Python
linktitle: Validieren Sie die Dateien XBRL und iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance Bibliothek API kann XBRL- und iXBRL-Dateien validieren. Weitere Informationen finden Sie in den Beispielcodes in diesem Artikel.
type: docs
weight: 30
url: /de/python-net/validate-xbrl-and-ixbrl-files/
---
## **Validieren Sie die Instanzdatei XBRL in Python**
 XBRL-Instanzen, XBRL-Linkbases und XBRL-Taxonomieschemata MÜSSEN den in[XBRL Spezifikation](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Um diese zu validieren, stellt die XbrlInstance-Klasse die Methode validate() bereit.

Das folgende Python-Code-Snippet zeigt, wie ein XBRL-Instanzdokument validiert wird.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **Validieren Sie die iXBRL-Datei in Python**
 Das[iXBRL Spezifikation](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html) definiert viele Validierungsregeln. Zum Validieren von iXBRL-Dateien stellt die InlineXbrlDocument-Klasse eine validate()-Methode bereit.

Das folgende Python-Code-Snippet veranschaulicht die Validierung eines iXBRL-Instanzdokuments.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **Validierungsfehlercodes**
 Im Enum ValidationErrorCode sind Validierungsfehlercodes für jede Validierungsregel definiert.
Im Folgenden sind die Definitionen der Fehlercodes aufgeführt:

- KONTEXT_ZEITRAUM_NEIN_ANFANG_ZEIT: Der Kontextzeitraumtyp ist Dauer, hat aber kein Startdatum.
- KONTEXT_ZEITRAUM_NEIN_ENDE_ZEIT: Der Kontextzeitraumtyp ist Dauer, hat aber kein Enddatum.
- KONTEXT_ZEITRAUM_ANFANG_NACH_ENDE: Der Kontextzeitraumtyp ist Dauer, aber das Enddatum liegt vor dem Startdatum.
- KONTEXT_SOFORTIG_NO_TIME: Der Kontextzeitraumtyp ist sofortig, hat aber kein sofortiges Datum.
- KONTEXT_SZENARIO_XBRL_NAMESPACE: Das Kontextszenario kann keinen XBRL-Namespace-Knoten haben.
- KONTEXT_SZENARIO_XBRL_AUSWECHSLUNG_GRUPPE: Das Kontextszenario darf kein Element in der Ersetzungsgruppe für Elemente haben, die im Namensraum XBRL definiert sind.
- KONTEXT_SZENARIO_LEER: Das Kontextszenario darf nicht leer sein.
- KONTEXT_SEGMENT_XBRL_NAMESPACE: Das Kontextsegment darf keinen XBRL-Namespace-Knoten haben.
- KONTEXT_SEGMENT_XBRL_SUBSTITUTIONGROUP: Das Kontextsegment darf kein Element in der Substitutionsgruppe für Elemente haben, die im Namensraum XBRL definiert sind.
- KONTEXT_SEGMENT_LEER: Kontextsegment darf nicht leer sein.
- ARTIKEL_NEIN_KONTEXT: Artikel muss einen Kontext haben.
- ARTIKEL_ZEITRAUM_TYP_KONFLIKT_WITH_CONTEXT: Artikel hat Periodentypkonflikt mit Kontext.
- ARTIKEL_NUMERISCH_NO_UNIT: Item ist numerisch und muss eine Einheit haben.
- GELD_ARTIKEL_NEIN_SINGLE_UNIT_MEASURE: Der Artikel ist ein Geldtyp und muss eine einzelne Maßeinheit haben.
- GELD_ARTIKEL_NO_ISO4217: Der Artikel ist ein Geldtyp und muss eine Maßeinheit im Stil von Iso 4217 haben.
- TEILEN_ARTIKEL_NEIN_SINGLE_UNIT_MEASURE: Artikel ist ein Anteilstyp und muss eine einzelne Maßeinheit haben.
- TEILEN_ARTIKEL_NEIN_TEILEN_UNIT_MEASURE: Der Artikel ist vom Typ „Share“ und muss eine xbrli:shares-Maßeinheit haben.
- NULL_ARTIKEL_MIT_PRÄZISION_OR_DECIMALS: Das Element ist null und darf weder Genauigkeit noch Dezimalstellen haben.
- FRAKTION_ARTIKEL_MIT_PRÄZISION_OR_DECIMALS: Item ist ein Bruchtyp und darf weder Genauigkeit noch Dezimalstellen haben.
- NUMERISCH_ARTIKEL_MIT_BEIDE_PRÄZISION_UND_DEZIMALS: Item ist ein numerischer Typ und darf nicht sowohl Genauigkeit als auch Dezimalstellen haben.
- NUMERISCH_ARTIKEL_OHNE_PRÄZISION_OR_DECIMALS: Item ist ein numerischer Typ und muss entweder Genauigkeit oder Dezimalstellen haben.
- NICHT_NUMERISCH_ARTIKEL_MIT_PRÄZISION_ODER_DEZIMALS: Item ist kein numerischer Typ und darf weder Genauigkeit noch Dezimalstellen haben.
- FUSSNOTE_BOGEN_AUS_NICHT_GEFUNDEN: Fußnotenbogen von Loc kann nicht gefunden werden.
- FUSSNOTE_BOGEN_ZU_NICHT_GEFUNDEN: Fußnotenbogen zu Fußnote kann nicht gefunden werden.
- DEFINITION_BOGEN_AUS_NICHT_GEFUNDEN: Definitionsbogen von Loc kann nicht gefunden werden.
- DEFINITION_BOGEN_ZU_NICHT_GEFUNDEN: Definitionsbogen zu Loc kann nicht gefunden werden.
- WESEN_ALIAS_DEFINITION_BOGEN_DIFFERENT_TYPE: Essence-Alias-Definitionsbogen hat verschiedene Typen.
- WESEN_ALIAS_DEFINITION_BOGEN_ANDERS_ZEITRAUM_TYPE: Essence-Alias Definition arc hat verschiedene periodTypes.
- WESEN_ALIAS_DEFINITION_BOGEN_DIFFERENT_BALANCE: Essence-Alias-Definitionsbogen hat unterschiedliche Balancen.
- BERECHNUNG_BOGEN_AUS_NICHT_GEFUNDEN: Berechnungsbogen von Loc.
- BERECHNUNG_BOGEN_ZU_NICHT_GEFUNDEN: Berechnungsbogen zu Loc kann nicht gefunden werden.
- ETIKETT_BOGEN_AUS_NICHT_GEFUNDEN: Lable arc von Loc kann nicht gefunden werden.
- ETIKETT_BOGEN_ZU_NICHT_GEFUNDEN: Lable Bogen zu Loc kann nicht gefunden werden.
- PRÄSENTATION_BOGEN_AUS_NICHT_GEFUNDEN: Präsentationsbogen von Loc.
- PRÄSENTATION_BOGEN_ZU_NICHT_GEFUNDEN: Präsentationsbogen zu Loc kann nicht gefunden werden.
- HINWEIS_BOGEN_AUS_NICHT_GEFUNDEN: Kein Referenzbogen von Loc.
- HINWEIS_BOGEN_ZU_NICHT_GEFUNDEN: Es konnte kein Referenzbogen zu Loc gefunden werden.
### **Beispiel für eine standardmäßige Validierungsfehlermeldung**
![todo: Bild_alt_Text](validate-xbrl-and-ixbrl-files_1.png)

Oben ist eine XBRL-Instanz, sie definiert den Kontext „cd1“, dieser Kontextzeitraumtyp ist Dauer, sein Startdatum ist 2002-03-31, das Enddatum ist 2001-03-31, also liegt das Enddatum vor dem Startdatum. In der XBRL-Spezifikation, Kapitel 4.7.2, definiert sie eine Validierungsregel: „das Enddatum MUSS einen Zeitpunkt spezifizieren oder implizieren, der nach dem angegebenen oder implizierten Zeitpunkt des entsprechenden Startdatums liegt“. Gemäß dieser Regel ist diese XBRL-Instanz nicht gültig.
## **XBRL validieren und Standardfehlermeldung ausgeben**
Der folgende Code validiert die Instanz XBRL und gibt die Standardfehlermeldung aus.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

Das folgende Bild zeigt die Ausgabe:

![todo: Bild_alt_Text](validate-xbrl-and-ixbrl-files_2.png)



