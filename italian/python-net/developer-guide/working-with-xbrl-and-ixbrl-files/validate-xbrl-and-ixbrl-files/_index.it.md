---
title: Convalida i file XBRL e iXBRL in Python
linktitle: Convalida i file XBRL e iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance La biblioteca API può convalidare i file XBRL e iXBRL. Consultare i codici di esempio forniti in questo articolo per ulteriori informazioni.
type: docs
weight: 30
url: /it/python-net/validate-xbrl-and-ixbrl-files/
---
## **Convalidare il file di istanza XBRL in Python**
 XBRL Istanze, XBRL Linkbase e XBRL Schemi di tassonomia DEVONO rispettare i requisiti di sintassi imposti in[XBRL specifica](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Per convalidarli, la classe XbrlInstance fornisce il metodo validate().

Il seguente frammento di codice Python illustra come convalidare un documento di istanza XBRL.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **Convalida il file iXBRL in Python**
 Il[iXBRL specifica](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html) definisce molte regole di convalida. Per la convalida dei file iXBRL, la classe InlineXbrlDocument fornisce un metodo validate().

Il seguente frammento di codice Python illustra la convalida di un documento di istanza iXBRL.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **Codici di errore di convalida**
 Nell'enumerazione ValidationErrorCode, i codici di errore di convalida sono definiti per ogni regola di convalida.
Di seguito sono riportate le definizioni dei codici di errore:

- CONTESTO_PERIODO_NO_INIZIO_TIME: il tipo di periodo del contesto è la durata, ma non ha una data di inizio.
- CONTESTO_PERIODO_NO_FINE_TIME: il tipo di periodo del contesto è la durata, ma non ha una data di fine.
- CONTESTO_PERIODO_INIZIO_DOPO_FINE: il tipo di periodo del contesto è la durata, ma la data di fine è precedente alla data di inizio.
- CONTESTO_IMMEDIATO_NO_TIME: il tipo di periodo del contesto è istantaneo, ma non ha una data istantanea.
- CONTESTO_SCENARIO_XBRL_NAMESPACE: lo scenario di contesto non può avere il nodo dello spazio dei nomi XBRL.
- CONTESTO_SCENARIO_XBRL_SOSTITUZIONE_GRUPPO: lo scenario di contesto non può avere un elemento nel gruppo di sostituzione per gli elementi definiti nello spazio dei nomi XBRL.
- CONTESTO_SCENARIO_EMPTY: lo scenario di contesto non può essere vuoto.
- CONTESTO_SEGMENTO_XBRL_NAMESPACE: il segmento di contesto non può avere il nodo dello spazio dei nomi XBRL.
- CONTESTO_SEGMENTO_XBRL_SUBSTITUTIONGROUP: il segmento di contesto non può avere un elemento nel gruppo di sostituzione per gli elementi definiti nello spazio dei nomi XBRL.
- CONTESTO_SEGMENTO_EMPTY: il segmento di contesto non può essere vuoto.
- ELEMENTO_NO_CONTESTO: l'elemento deve avere un contesto.
- ELEMENTO_PERIODO_GENERE_CONFLITTO_WITH_CONTEXT: l'elemento presenta un conflitto di tipo di periodo con il contesto.
- ELEMENTO_NUMERICO_NO_UNIT: l'elemento è numerico e deve avere un'unità.
- MONETARIO_ELEMENTO_NO_SEPARARE_UNIT_MEASURE: l'articolo è di tipo monetario e deve avere una singola unità di misura.
- MONETARIO_ELEMENTO_NO_ISO4217: l'articolo è di tipo monetario e deve avere un'unità di misura in stile Iso 4217.
- CONDIVIDERE_ELEMENTO_NO_SEPARARE_UNIT_MEASURE: l'articolo è un tipo di condivisione e deve avere una singola unità di misura.
- CONDIVIDERE_ELEMENTO_NO_CONDIVIDERE_UNIT_MEASURE: l'elemento è di tipo condiviso e deve avere un'unità di misura xbrli:shares.
- NULLO_ELEMENTO_INSIEME A_PRECISIONE_OR_DECIMALS: l'elemento è nullo e non deve avere né precisione né decimali.
- FRAZIONE_ELEMENTO_INSIEME A_PRECISIONE_OR_DECIMALS: l'elemento è un tipo di frazione e non deve avere né precisione né decimali.
- NUMERICO_ELEMENTO_INSIEME A_ENTRAMBI_PRECISIONE_E_DECIMALI: l'elemento è di tipo numerico e non deve avere sia precisione che decimali.
- NUMERICO_ELEMENTO_SENZA_PRECISIONE_OR_DECIMALS: l'elemento è di tipo numerico e deve avere precisione o decimali.
- NON_NUMERICO_ELEMENTO_INSIEME A_PRECISIONE_O_DECIMALI: l'elemento non è un tipo numerico e non deve avere né precisione né decimali.
- NOTA_ARCO_DA_NON_TROVATO: Impossibile trovare l'arco delle note a piè di pagina da Loc.
- NOTA_ARCO_A_NON_TROVATO: impossibile trovare l'arco della nota a piè di pagina nella nota a piè di pagina.
- DEFINIZIONE_ARCO_DA_NON_TROVATO: Impossibile trovare l'arco di definizione da Loc.
- DEFINIZIONE_ARCO_A_NON_TROVATO: Impossibile trovare l'arco di definizione in Loc.
- ESSENZA_ALIAS_DEFINIZIONE_ARCO_DIFFERENT_TYPE: Essence-alias Definition arc ha diversi tipi.
- ESSENZA_ALIAS_DEFINIZIONE_ARCO_DIVERSO_PERIODO_TIPO: Essence-alias Definition arc ha diversi periodTypes.
- ESSENZA_ALIAS_DEFINIZIONE_ARCO_DIFFERENT_BALANCE: Essence-alias Definition arc ha diversi saldi.
- CALCOLO_ARCO_DA_NON_TROVATO: Impossibile trovare l'arco di calcolo da Loc.
- CALCOLO_ARCO_A_NON_TROVATO: impossibile trovare l'arco di calcolo a Loc.
- ETICHETTA_ARCO_DA_NON_TROVATO: Impossibile trovare Lable arc da Loc.
- ETICHETTA_ARCO_A_NON_TROVATO: Impossibile trovare Lable arc to Loc.
- PRESENTAZIONE_ARCO_DA_NON_TROVATO: impossibile trovare un arco di presentazione da Loc.
- PRESENTAZIONE_ARCO_A_NON_TROVATO: impossibile trovare un arco di presentazione a Loc.
- RIFERIMENTO_ARCO_DA_NON_FOUND: Impossibile trovare un arco di riferimento da Loc.
- RIFERIMENTO_ARCO_A_NON_TROVATO: impossibile trovare un arco di riferimento a Loc.
### **Esempio di messaggio di errore di convalida standard**
![cose da fare:immagine_alt_testo](validate-xbrl-and-ixbrl-files_1.png)

Sopra c'è un'istanza XBRL, definisce il contesto "cd1", questo tipo di periodo di contesto è la durata, la sua data di inizio è 2002-03-31, la data di fine è 2001-03-31, quindi la data di fine è precedente alla data di inizio. Nella specifica XBRL, capitolo 4.7.2, definisce la regola di convalida: "la data di fine DEVE specificare o implicare un punto nel tempo che è successivo al punto nel tempo specificato o implicito della corrispondente data di inizio". Secondo questa regola, questa istanza XBRL non è valida.
## **Convalidare XBRL e generare un messaggio di errore standard**
Il codice seguente convalida l'istanza XBRL e restituisce il messaggio di errore standard.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

L'immagine seguente mostra l'output:

![cose da fare:immagine_alt_testo](validate-xbrl-and-ixbrl-files_2.png)



