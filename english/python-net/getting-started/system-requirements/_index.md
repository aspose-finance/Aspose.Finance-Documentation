---
title: System Requirements
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /python-net/system-requirements/
description: Learn about System Requirements of Python Finance Library API 
---

## **Supported Operating Systems**
### **Windows**
- Microsoft Windows 2000 ( x64, x86)
- Microsoft Windows XP ( x64, x86)
- Microsoft Windows Server 2003 ( x64, x86)
- Microsoft Windows Server 2008 ( x64, x86)
- Microsoft Windows Server 2012 ( x64, x86)
- Microsoft Windows Vista ( x64, x86)
- Microsoft Windows 7 ( x64, x86)
- Microsoft Windows 8 ( x64, x86)
- Microsoft Windows 10 ( x64, x86)
### **Linux**
- Ubuntu
- OpenSUSE
- CentOS
- and others

## System Requirements for Target Linux Platform

- GCC-6 runtime libraries (or later).

- Dependencies of .NET Core Runtime. Installing .NET Core Runtime itself is NOT required.

- For Python 3.5-3.7: The `pymalloc` build of Python is needed. The `--with-pymalloc` Python build option is enabled by default. Typically, the `pymalloc` build of Python is marked with `m` suffix in the filename.

- `libpython` shared Python library. The `--enable-shared` Python build option is disabled by default, some Python distributions do not contain the `libpython` shared library. For some linux platforms, the `libpython` shared library can be installed using the package manager, for example: `sudo apt-get install libpython3.7`. The common issue is that `libpython` library is installed in a different location than the standard system location for shared libraries. The issue can be fixed by using the Python build options to set alternate library paths when compiling Python, or fixed by creating a symbolic link to the `libpython` library file in the system standard location for shared libraries. Typically, the `libpython` shared library file name is `libpythonX.Ym.so.1.0` for Python 3.5-3.7, or `libpythonX.Y.so.1.0` for Python 3.8 or later (for example: libpython3.7m.so.1.0, libpython3.9.so.1.0).
