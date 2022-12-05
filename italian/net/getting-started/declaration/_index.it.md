---
title: Dichiarazione
type: docs
weight: 30
url: /it/net/declaration/
---
## **Sfida fiducia parziale/fiducia media**
Tutti i componenti Aspose .NET richiedono il set di autorizzazioni Full Trust. Il motivo è che i componenti Aspose .NET devono accedere alle impostazioni del registro, ai file di sistema diversi da una directory virtuale per determinate operazioni come l'analisi dei caratteri, ecc. casi.

I provider di servizi Internet che ospitano più applicazioni di società diverse applicano principalmente il livello di sicurezza Medium Trust. Nel caso di .NET 2.0, tale livello di sicurezza applica i seguenti vincoli:

- · **Autorizzazione OleDb** Non è disponibile. Ciò significa che non è possibile utilizzare il provider di dati OLE DB gestito ADO.NET per accedere ai database.
- · **EventLogPermission** Non è disponibile. Ciò significa che non è possibile accedere al registro eventi Windows.
- · **ReflectionPermission** Non è disponibile. Ciò significa che non puoi usare la riflessione.
- · **RegistryPermission** Non è disponibile. Ciò significa che non è possibile accedere al registro.
- · **Autorizzazione Web** è limitato. Ciò significa che la tua applicazione può comunicare solo con un indirizzo o un intervallo di indirizzi che definisci nel file<trust> elemento.
- · **FileIOPermission** è limitato. Ciò significa che puoi accedere solo ai file nella gerarchia di directory virtuale della tua applicazione.

Per i motivi sopra specificati, i componenti Aspose .NET non possono essere utilizzati su server che concedono set di autorizzazioni diversi da Full Trust.
