---
title: Licenza
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /it/python-net/licensing/
description: Python Finance La biblioteca API invita i suoi clienti a ottenere una licenza classica e una licenza a consumo. Oltre a utilizzare una licenza limitata per esplorare meglio il prodotto.
---
volte, per studiare meglio il sistema, vuoi immergerti nel codice il più velocemente possibile. Per rendere tutto più semplice, Aspose.Finance fornisce diversi piani per l'acquisto o offre una prova gratuita e una licenza temporanea di 30 giorni per la valutazione.

{{% alert color="primary" %}}

 Tieni presente che esistono una serie di politiche e pratiche generali che ti guidano su come valutare, concedere in licenza correttamente e acquistare i nostri prodotti. Li puoi trovare nel["Politiche di acquisto e FAQ"](https://purchase.aspose.com/policies) sezione.

{{% /alert %}}

## **Valuta Aspose.Finance**
 Puoi facilmente scaricare Aspose.Finance per la valutazione. Il pacchetto di valutazione è lo stesso del pacchetto acquistato. La versione di valutazione ottiene semplicemente la licenza dopo aver aggiunto alcune righe di codice per applicare la licenza.

### **Limiti della versione di valutazione**
La versione di valutazione fornisce tutte le funzionalità tranne le seguenti:

- **Numero di file aperti** (Aspose.Finance) Quando si esegue il programma, è possibile aprire solo 50 file utilizzando la libreria Aspose.Finance. Se la tua applicazione supera questo numero, verrà generata un'eccezione.
- **Numero di file salvati** (Aspose.Finance) Quando si esegue il programma, è possibile aprire solo 50 file utilizzando la libreria Aspose.Finance. Se la tua applicazione supera questo numero, verrà generata un'eccezione.

{{% alert color="primary" %}} 

 Se vuoi provare Aspose.Finance senza limiti di valutazione, richiedi una licenza temporanea di 30 giorni. Per favore riferisci a[Come ottenere una licenza temporanea?](https://purchase.aspose.com/temporary-license) per maggiori informazioni.

{{% /alert %}} 

## **Informazioni sulla licenza**
 Puoi facilmente scaricare una versione di valutazione di Aspose.Finance per Python tramite .NET dal suo[pagina di download](https://pypi.org/project/aspose.finance/) . La versione di valutazione fornisce assolutamente**le stesse capacità**come versione con licenza di Aspose.Finance. Inoltre, la versione di valutazione diventa semplicemente concessa in licenza dopo aver acquistato una licenza e aver aggiunto un paio di righe di codice per applicare la licenza.

La licenza è un file XML di testo semplice che contiene dettagli come il nome del prodotto, il numero di sviluppatori a cui è concesso in licenza, la data di scadenza dell'abbonamento e così via. Il file è firmato digitalmente, quindi non modificarlo. Anche un'aggiunta involontaria di un'ulteriore interruzione di riga al contenuto del file lo invaliderà.

 Per evitare le limitazioni associate alla versione di valutazione, è necessario impostare una licenza prima dell'utilizzo**Aspose.Finance**. È necessario impostare una licenza solo una volta per applicazione o processo.

## Licenza acquistata

Dopo l'acquisto, è necessario applicare il file di licenza o lo streaming. Questa sezione descrive le opzioni su come farlo e commenta anche alcune domande comuni.

{{% alert color="primary" %}}

Devi impostare la licenza:
* una sola volta per dominio dell'applicazione
* prima di utilizzare qualsiasi altra classe Aspose.Finance

{{% /alert %}}

{{% alert color="primary" %}}

È possibile trovare informazioni sui prezzi su["Informazioni sui prezzi"](https://purchase.aspose.com/pricing/finance/family) pagina.

{{% /alert %}}

### **Impostazione di una licenza in Aspose.Finance per Python tramite .NET**

Le licenze possono essere applicate da varie località:

* Percorso esplicito
* La cartella contenente lo script python che chiama Aspose.Finance per Python tramite .NET
* Flusso
* Come licenza a consumo: un nuovo meccanismo di licenza

{{% alert color="primary" %}}

 Utilizzare il**set_licenza** metodo per concedere in licenza un componente.

 Chiamata**set_licenza** più volte non è dannoso, fa solo perdere tempo al processore.

{{% /alert %}}

 Nelle sezioni seguenti, descriveremo i due metodi comuni utilizzati per impostare la licenza.

#### **Applicazione di una licenza utilizzando un file**
Il metodo più semplice per impostare una licenza richiede di posizionare il file di licenza nella stessa cartella contenente lo script python che chiama Aspose.Finance per Python e specificare solo il nome del file senza il relativo percorso.

Questo frammento di codice viene utilizzato per impostare un file di licenza:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

Quando si chiama il metodo set_license, il nome della licenza deve essere uguale a quello del file di licenza. Ad esempio, è possibile modificare il nome del file di licenza in "Aspose.Finance.lic.xml". Quindi, nel tuo codice, devi passare il nuovo nome di licenza (Aspose.Finance.lic.xml) al metodo SetLicense.

#### **Applicazione di una licenza da un flusso**
 Puoi caricare una licenza da un flusso.

Questo frammento di codice viene utilizzato per applicare una licenza da uno stream:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Applicare la licenza misurata

Aspose.Finance consente agli sviluppatori di applicare una chiave a consumo. Questo è un nuovo meccanismo di licenza.

Il nuovo meccanismo di licenza verrà utilizzato insieme al metodo di licenza esistente. I clienti che desiderano essere fatturati in base all'utilizzo delle funzionalità API possono utilizzare la licenza misurata.

 Dopo aver completato tutti i passaggi necessari per ottenere questo tipo di licenza, riceverai le chiavi, non il file di licenza. Questa chiave misurata può essere applicata utilizzando il**Misurato** classe appositamente introdotta per questo scopo.

L'esempio di codice seguente mostra come impostare chiavi pubbliche e private misurate:

```py
import aspose.finance as af

# Create an instance of CAD Metered class
metered = af.Metered()

# Access the set_metered_key property and pass public and private keys as parameters
metered.set_metered_key("*****", "*****")

# Get metered data amount before calling API
amountbefore = metered.get_consumption_quantity()
# Display information
print("Amount Consumed Before: " + str(amountbefore))

# handle finance file
# ......

# Get metered data amount After calling API
amountafter = metered.get_consumption_quantity()
# Display information
print("Amount Consumed After: " + str(amountafter))
```

{{% alert color="primary" %}}

 Si prega di notare che è necessario disporre di una connessione Internet stabile per il corretto utilizzo della licenza Metered, poiché il meccanismo Metered richiede l'interazione costante con i nostri servizi per calcoli corretti. Per maggiori dettagli, consultare il["Domande frequenti sulle licenze misurate"](https://purchase.aspose.com/faqs/licensing/metered) sezione.

{{% /alert %}}
