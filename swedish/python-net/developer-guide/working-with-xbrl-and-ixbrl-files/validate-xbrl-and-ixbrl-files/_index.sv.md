---
title: Validera filerna XBRL och iXBRL i Python
linktitle: Validera filerna XBRL och iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance Bibliotek API kan validera XBRL och iXBRL filer. Se exempelkoderna i den här artikeln för mer information.
type: docs
weight: 30
url: /sv/python-net/validate-xbrl-and-ixbrl-files/
---
## **Validera instansfilen XBRL i Python**
 XBRL Instances, XBRL Linkbases och XBRL Taxonomy Schemas MÅSTE uppfylla syntaxkraven i[XBRL specifikation](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). För att validera dessa tillhandahåller klassen XbrlInstance metoden validate().

Följande Python-kodavsnitt visar hur man validerar ett XBRL-instansdokument.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **Validera filen iXBRL i Python**
 De[iXBRL specifikation](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html) definierar många valideringsregler. För validering av iXBRL-filer tillhandahåller klassen InlineXbrlDocument en validate()-metod.

Följande Python-kodavsnitt visar validering av ett iXBRL-instansdokument.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **Validering felkoder**
 I enum ValidationErrorCode definieras valideringsfelkoder för varje valideringsregel.
Följande är felkodsdefinitionerna:

- SAMMANHANG_PERIOD_NEJ_START_TID: Typ av kontextperiod är varaktighet, men har inget startdatum.
- SAMMANHANG_PERIOD_NEJ_SLUTET_TID: Typ av kontextperiod är varaktighet, men har inget slutdatum.
- SAMMANHANG_PERIOD_START_EFTER_SLUT: Typ av kontextperiod är varaktighet, men slutdatumet är före startdatumet.
- SAMMANHANG_OMEDELBAR_NO_TIME: Typ av kontextperiod är omedelbar, men har inget direktdatum.
- SAMMANHANG_SCENARIO_XBRL_NAMESPACE: Kontextscenariot kan inte ha XBRL namnområdesnod.
- SAMMANHANG_SCENARIO_XBRL_UTBYTE_GROUP: Kontextscenariot kan inte ha ett element i ersättningsgruppen för element definierade i namnområdet XBRL.
- SAMMANHANG_SCENARIO_TOM: Kontextscenariot kan inte vara tomt.
- SAMMANHANG_SEGMENTET_XBRL_NAMESPACE: Kontextsegment kan inte ha XBRL namnområdesnod.
- SAMMANHANG_SEGMENTET_XBRL_SUBSTITUTIONGROUP: Kontextsegment kan inte ha element i ersättningsgruppen för element definierade i namnområdet XBRL.
- SAMMANHANG_SEGMENTET_TOM: Kontextsegmentet får inte vara tomt.
- ARTIKEL_NEJ_KONTEXT: Objektet måste ha ett sammanhang.
- ARTIKEL_PEROID_TYP_KONFLIKT_WITH_CONTEXT: Objektet har periodtyp i konflikt med sammanhanget.
- ARTIKEL_NUMERISK_NO_UNIT: Objektet är numeriskt och måste ha en enhet.
- MONETÄR_ARTIKEL_NEJ_ENDA_UNIT_MEASURE: Objekt är en monetär typ och måste ha ett enda mått.
- MONETÄR_ARTIKEL_NO_ISO4217: Föremålet är en monetär typ och måste ha ett enhetsmått i Iso 4217-stil.
- DELA MED SIG_ARTIKEL_NEJ_ENDA_UNIT_MEASURE: Objektet är en andelstyp och måste ha ett enda mått.
- DELA MED SIG_ARTIKEL_NEJ_DELA MED SIG_UNIT_MEASURE: Objektet är delningstyp och måste ha ett xbrli:shares enhetsmått.
- NILL_ARTIKEL_MED_PRECISION_OR_DECIMALS: Artikeln är noll och får inte ha vare sig precision eller decimaler.
- FRAKTION_ARTIKEL_MED_PRECISION_OR_DECIMALS: Objekt är en bråktyp och får inte ha vare sig precision eller decimaler.
- NUMERISK_ARTIKEL_MED_BÅDE_PRECISION_OCH_DECIMALER: Objektet är en numerisk typ och får inte ha både precision och decimaler.
- NUMERISK_ARTIKEL_UTAN_PRECISION_OR_DECIMALS: Objektet är en numerisk typ och måste ha antingen precision eller decimaler.
- EJ_NUMERISK_ARTIKEL_MED_PRECISION_ELLER_DECIMALER: Objektet är inte en numerisk typ och får inte ha vare sig precision eller decimaler.
- FOTNOT_BÅGE_FRÅN_INTE_FOUND: Det gick inte att hitta fotnotsbågen från Loc.
- FOTNOT_BÅGE_TILL_INTE_FOUND: Det gick inte att hitta fotnotsbåge till fotnot.
- DEFINITION_BÅGE_FRÅN_INTE_FOUND: Det gick inte att hitta definitionsbågen från Loc.
- DEFINITION_BÅGE_TILL_INTE_FOUND: Det gick inte att hitta definitionsbågen till Loc.
- VÄSEN_ALIAS_DEFINITION_BÅGE_DIFFERENT_TYPE: Essence-alias Definition arc har olika typer.
- VÄSEN_ALIAS_DEFINITION_BÅGE_ANNORLUNDA_PERIOD_TYPE: Essence-alias Definition arc har olika periodTypes.
- VÄSEN_ALIAS_DEFINITION_BÅGE_DIFFERENT_BALANCE: Essence-alias Definition arc har olika balanser.
- BERÄKNING_BÅGE_FRÅN_INTE_FOUND: Det gick inte att hitta beräkningsbåge från Loc.
- BERÄKNING_BÅGE_TILL_INTE_FOUND: Det gick inte att hitta beräkningsbågen till Loc.
- MÄRKA_BÅGE_FRÅN_INTE_FOUND: Det gick inte att hitta Lable-bågen från Loc.
- MÄRKA_BÅGE_TILL_INTE_FOUND: Det gick inte att hitta Lable arc to Loc.
- PRESENTATION_BÅGE_FRÅN_INTE_FOUND: Det gick inte att hitta en presentationsbåge från Loc.
- PRESENTATION_BÅGE_TILL_INTE_FOUND: Det gick inte att hitta en presentationsbåge till Loc.
- REFERENS_BÅGE_FRÅN_INTE_FOUND: Det gick inte att hitta en referensbåge från Loc.
- REFERENS_BÅGE_TILL_INTE_FOUND: Det gick inte att hitta en referensbåge till Loc.
### **Exempel på standard valideringsfelmeddelande**
![todo:image_alt_text](validate-xbrl-and-ixbrl-files_1.png)

Ovan är en XBRL-instans, den definierar sammanhanget "cd1", denna kontextperiodtyp är varaktighet, dess startdatum är 2002-03-31, slutdatumet är 2001-03-31, så slutdatumet är före startdatumet. I XBRL-specifikationen, kapitel 4.7.2, definierar den valideringsregeln: "slutdatumet MÅSTE ange eller antyda en tidpunkt som är senare än den angivna eller underförstådda tidpunkten för motsvarande startdatum". Enligt denna regel är denna XBRL-instans inte en giltig.
## **Validera XBRL och mata ut standardfelmeddelande**
Följande kod validerar XBRL-instansen och matar ut standardfelmeddelandet.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

Följande bild visar resultatet:

![todo:image_alt_text](validate-xbrl-and-ixbrl-files_2.png)



