---
title: Systemkrav
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /sv/python-net/system-requirements/
description:  Lär dig mer om systemkrav för Python Finance Bibliotek API
---
## **Operativsystem som stöds**
### **Windows**
- Microsoft Windows 2000 ( x64, x86)
- Microsoft Windows XP ( x64, x86)
- Microsoft Windows Server 2003 ( x64, x86)
- Microsoft Windows Server 2008 ( x64, x86)
- Microsoft Windows Server 2012 ( x64, x86)
- Microsoft Windows Vista ( x64, x86)
- Microsoft Windows 7 ( x64, x86)
- Microsoft Windows 8 ( x64, x86)
- Microsoft Windows 10 ( x64, x86)
### **Linux**
- Ubuntu
- OpenSUSE
- CentOS
- och andra

## Systemkrav för Target Linux Platform

- GCC-6 runtime-bibliotek (eller senare).

- Beroenden av .NET Core Runtime. Installation av själva .NET Core Runtime krävs INTE.

- För Python 3.5-3.7: `pymalloc`-bygget av Python behövs. Byggalternativet `--with-pymalloc` Python är aktiverat som standard. Vanligtvis är `pymalloc` build av Python märkt med `m` suffix i filnamnet.

- `libpython` delat Python bibliotek. Byggalternativet `--enable-shared` Python är inaktiverat som standard, vissa Python-distributioner innehåller inte det delade biblioteket `libpython`. För vissa Linux-plattformar kan det delade biblioteket `libpython` installeras med hjälp av pakethanteraren, till exempel: `sudo apt-get install libpython3.7`. Det vanliga problemet är att biblioteket `libpython` är installerat på en annan plats än standardsystemplatsen för delade bibliotek. Problemet kan åtgärdas genom att använda byggalternativen Python för att ställa in alternativa bibliotekssökvägar vid kompilering av Python, eller fixas genom att skapa en symbolisk länk till biblioteksfilen `libpython` på systemets standardplats för delade bibliotek. Vanligtvis är filnamnet för `libpython` delat bibliotek `libpythonX.Ym.so.1.0` för Python 3.5-3.7, eller `libpythonX.Y.so.1.0` för Python 3.8 eller senare (till exempel: libpython.1.0m.0m.1.0m.1.0m.9).
