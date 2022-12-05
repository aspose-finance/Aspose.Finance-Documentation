---
title: Requisitos del sistema
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /es/python-net/system-requirements/
description:  Más información sobre los requisitos del sistema de la biblioteca Python Finance API
---
## **Sistemas operativos compatibles**
### **Windows**
- Microsoft Windows 2000 (x64, x86)
- Microsoft Windows EXP (x64, x86)
- Microsoft Windows Servidor 2003 (x64, x86)
- Microsoft Windows Servidor 2008 (x64, x86)
- Microsoft Windows Servidor 2012 (x64, x86)
- Microsoft Windows Vista (x64, x86)
- Microsoft Windows 7 (x64, x86)
- Microsoft Windows 8 (x64, x86)
- Microsoft Windows 10 (x64, x86)
### **linux**
- ubuntu
- abrirSUSE
- CentOS
- y otros

## Requisitos del sistema para la plataforma Linux de destino

- Bibliotecas de tiempo de ejecución GCC-6 (o posterior).

- Dependencias de .NET Core Runtime. NO es necesario instalar .NET Core Runtime.

- Para Python 3.5-3.7: se necesita la compilación `pymalloc` de Python. La opción de compilación `--with-pymalloc` Python está habilitada de manera predeterminada. Por lo general, la compilación `pymalloc` de Python está marcada con el sufijo `m` en el nombre del archivo.

- `libpython` biblioteca compartida Python. La opción de compilación `--enable-shared` Python está deshabilitada de forma predeterminada, algunas distribuciones Python no contienen la biblioteca compartida `libpython`. Para algunas plataformas Linux, la biblioteca compartida `libpython` se puede instalar usando el administrador de paquetes, por ejemplo: `sudo apt-get install libpython3.7`. El problema común es que la biblioteca `libpython` está instalada en una ubicación diferente a la ubicación estándar del sistema para bibliotecas compartidas. El problema se puede solucionar usando las opciones de compilación Python para establecer rutas de biblioteca alternativas al compilar Python, o se puede solucionar creando un enlace simbólico al archivo de biblioteca `libpython` en la ubicación estándar del sistema para bibliotecas compartidas. Normalmente, el nombre del archivo de la biblioteca compartida `libpython` es `libpythonX.Ym.so.1.0` para Python 3.5-3.7 o `libpythonX.Y.so.1.0` para Python 3.8 o posterior (por ejemplo: libpython3.7m.so.1.0, libpython3.9.so.1.0).
