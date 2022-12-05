---
title: Requisiti di sistema
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /it/python-net/system-requirements/
description:  Informazioni sui requisiti di sistema della libreria Python Finance API
---
## **Sistemi operativi supportati**
### **Windows**
- Microsoft Windows 2000 (x64, x86)
- Microsoft Windows XP (x64, x86)
- Microsoft Windows Server 2003 (x64, x86)
- Microsoft Windows Server 2008 (x64, x86)
- Microsoft Windows Server 2012 (x64, x86)
- Microsoft Windows Vista (x64, x86)
- Microsoft Windows 7 (x64, x86)
- Microsoft Windows 8 (x64, x86)
- Microsoft Windows 10 (x64, x86)
### **Linux**
- Ubuntu
- OpenSUSE
- CentOS
- e altri

## Requisiti di sistema per la piattaforma Linux di destinazione

- Librerie di runtime GCC-6 (o successive).

- Dipendenze di .NET Core Runtime. L'installazione di .NET Core Runtime NON è richiesta.

- Per Python 3.5-3.7: è necessaria la build `pymalloc` di Python. L'opzione di compilazione `--with-pymalloc` Python è abilitata per impostazione predefinita. In genere, la build `pymalloc` di Python è contrassegnata con il suffisso `m` nel nome del file.

- `libpython` biblioteca condivisa Python. L'opzione di compilazione `--enable-shared` Python è disabilitata per impostazione predefinita, alcune distribuzioni Python non contengono la libreria condivisa `libpython`. Per alcune piattaforme Linux, la libreria condivisa `libpython` può essere installata utilizzando il gestore pacchetti, ad esempio: `sudo apt-get install libpython3.7`. Il problema comune è che la libreria `libpython` è installata in una posizione diversa rispetto alla posizione di sistema standard per le librerie condivise. Il problema può essere risolto utilizzando le opzioni di compilazione Python per impostare percorsi di libreria alternativi durante la compilazione di Python o risolto creando un collegamento simbolico al file di libreria `libpython` nella posizione standard del sistema per le librerie condivise. In genere, il nome del file della libreria condivisa `libpython` è `libpythonX.Ym.so.1.0` per Python 3.5-3.7 o `libpythonX.Y.so.1.0` per Python 3.8 o successivo (ad esempio: libpython3.7m.so.1.0, libpython3.9.so.1.0).
