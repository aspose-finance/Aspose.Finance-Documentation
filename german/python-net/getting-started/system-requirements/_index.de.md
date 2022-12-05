---
title: System Anforderungen
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /de/python-net/system-requirements/
description:  Erfahren Sie mehr über die Systemanforderungen der Bibliothek Python Finance API
---
## **Unterstützte Betriebssysteme**
### **Windows**
- Microsoft Windows 2000 ( x64, x86)
- Microsoft Windows XP (x64, x86)
- Microsoft Windows Server 2003 (x64, x86)
- Microsoft Windows Server 2008 (x64, x86)
- Microsoft Windows Server 2012 (x64, x86)
- Microsoft Windows Vista (x64, x86)
- Microsoft Windows 7 ( x64, x86)
- Microsoft Windows 8 ( x64, x86)
- Microsoft Windows 10 ( x64, x86)
### **Linux**
- Ubuntu
- OpenSUSE
- CentOS
- und andere

## Systemanforderungen für die Ziel-Linux-Plattform

- GCC-6-Laufzeitbibliotheken (oder höher).

- Abhängigkeiten von .NET Core Runtime. Die Installation von .NET Core Runtime selbst ist NICHT erforderlich.

- Für Python 3.5-3.7: Der Build `pymalloc` von Python wird benötigt. Die Build-Option `--with-pymalloc` Python ist standardmäßig aktiviert. Normalerweise ist der Build `pymalloc` von Python mit dem Suffix `m` im Dateinamen gekennzeichnet.

- `libpython` gemeinsam genutzte Python Bibliothek. Die Build-Option `--enable-shared` Python ist standardmäßig deaktiviert, einige Python-Distributionen enthalten die gemeinsam genutzte `libpython`-Bibliothek nicht. Für einige Linux-Plattformen kann die gemeinsam genutzte Bibliothek `libpython` mithilfe des Paketmanagers installiert werden, zum Beispiel: `sudo apt-get install libpython3.7`. Das häufige Problem besteht darin, dass die Bibliothek `libpython` an einem anderen Speicherort als dem Standardsystemspeicherort für gemeinsam genutzte Bibliotheken installiert wird. Das Problem kann behoben werden, indem die Python-Erstellungsoptionen verwendet werden, um beim Kompilieren von Python alternative Bibliothekspfade festzulegen, oder indem ein symbolischer Link zur Bibliotheksdatei `libpython` im Systemstandardspeicherort für gemeinsam genutzte Bibliotheken erstellt wird. Normalerweise lautet der Dateiname der gemeinsam genutzten Bibliothek `libpython` `libpythonX.Ym.so.1.0` für Python 3.5-3.7 oder `libpythonX.Y.so.1.0` für Python 3.8 oder höher (z. B.: libpython3.7m.so.1.0, libpython3.9.so.1.0).
