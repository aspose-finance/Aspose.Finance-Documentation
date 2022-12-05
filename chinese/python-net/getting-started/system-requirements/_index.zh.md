---
title: 系统要求
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /zh/python-net/system-requirements/
description: 了解 Python Finance 库 API 的系统要求
---
## **支持的操作系统**
### **Windows**
- Microsoft Windows 2000（x64，x86）
- Microsoft Windows XP（x64、x86）
- Microsoft Windows 服务器 2003（x64、x86）
- Microsoft Windows 服务器 2008（x64、x86）
- Microsoft Windows 服务器 2012（x64、x86）
- Microsoft Windows Vista（x64、x86）
- Microsoft Windows 7（x64，x86）
- Microsoft Windows 8（x64，x86）
- Microsoft Windows 10（x64，x86）
### **Linux**
- Ubuntu
- 开放SUSE
- 中央操作系统
- 和别的

## 目标 Linux 平台的系统要求

- GCC-6 运行时库（或更高版本）。

- .NET 核心运行时的依赖项。不需要安装 .NET Core Runtime 本身。

- 对于 Python 3.5-3.7：需要 Python 的 `pymalloc` 版本。默认启用 `--with-pymalloc` Python 构建选项。通常，Python 的 `pymalloc` 版本在文件名中标有 `m` 后缀。

- `libpython` 共享 Python 库。 `--enable-shared` Python 构建选项默认禁用，一些 Python 发行版不包含 `libpython` 共享库。对于某些 linux 平台，可以使用包管理器安装 `libpython` 共享库，例如：`sudo apt-get install libpython3.7`。常见的问题是 `libpython` 库安装在与共享库的标准系统位置不同的位置。该问题可以通过在编译 Python 时使用 Python 构建选项设置备用库路径来解决，或者通过在共享库的系统标准位置创建指向 `libpython` 库文件的符号链接来解决。通常，`libpython` 共享库文件名对于 Python 3.5-3.7 为 `libpythonX.Ym.so.1.0`，对于 Python 3.8 或更高版本为 `libpythonX.Y.so.1.0`（例如：libpython3.7m.so.1.0、libpython3.9.so.1.0）。
