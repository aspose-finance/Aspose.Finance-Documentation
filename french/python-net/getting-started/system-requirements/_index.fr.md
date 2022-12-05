---
title: Configuration requise
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /fr/python-net/system-requirements/
description:  En savoir plus sur la configuration système requise de la bibliothèque Python Finance API
---
## **Systèmes d'exploitation pris en charge**
### **Windows**
- Microsoft Windows 2000 (x64, x86)
- Microsoft Windows XP (x64, x86)
- Microsoft Windows Serveur 2003 (x64, x86)
- Microsoft Windows Serveur 2008 (x64, x86)
- Microsoft Windows Serveur 2012 (x64, x86)
- Microsoft Windows Vista (x64, x86)
- Microsoft Windows 7 (x64, x86)
- Microsoft Windows 8 (x64, x86)
- Microsoft Windows 10 (x64, x86)
### **Linux**
- Ubuntu
- OuvrirSUSE
- CentOS
- et d'autres

## Configuration système requise pour la plate-forme Linux cible

- Bibliothèques d'exécution GCC-6 (ou ultérieures).

- Dépendances de .NET Core Runtime. L'installation de .NET Core Runtime n'est PAS nécessaire.

- Pour Python 3.5-3.7 : La version `pymalloc` de Python est nécessaire. L'option de construction `--with-pymalloc` Python est activée par défaut. En règle générale, la version `pymalloc` de Python est marquée du suffixe `m` dans le nom de fichier.

- `libpython` bibliothèque partagée Python. L'option de construction `--enable-shared` Python est désactivée par défaut, certaines distributions Python ne contiennent pas la bibliothèque partagée `libpython`. Pour certaines plates-formes Linux, la bibliothèque partagée `libpython` peut être installée à l'aide du gestionnaire de packages, par exemple : `sudo apt-get install libpython3.7`. Le problème courant est que la bibliothèque `libpython` est installée à un emplacement différent de l'emplacement système standard pour les bibliothèques partagées. Le problème peut être résolu en utilisant les options de construction Python pour définir des chemins de bibliothèque alternatifs lors de la compilation de Python, ou en créant un lien symbolique vers le fichier de bibliothèque `libpython` dans l'emplacement standard du système pour les bibliothèques partagées. Généralement, le nom du fichier de bibliothèque partagée `libpython` est `libpythonX.Ym.so.1.0` pour Python 3.5-3.7, ou `libpythonX.Y.so.1.0` pour Python 3.8 ou version ultérieure (par exemple : libpython3.7m.so.1.0, libpython3.9.so.1.0).
