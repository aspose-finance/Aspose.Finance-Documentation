---
title: Системные Требования
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /ru/python-net/system-requirements/
description:  Узнайте о системных требованиях библиотеки Python Finance API
---
## **Поддерживаемые операционные системы**
### **Windows**
- Microsoft Windows 2000 (x64, x86)
- Microsoft Windows XP (x64, x86)
- Microsoft Windows Сервер 2003 (x64, x86)
- Microsoft Windows Сервер 2008 (x64, x86)
- Microsoft Windows Сервер 2012 (x64, x86)
- Microsoft Windows Перспектива (x64, x86)
- Microsoft Windows 7 ( х64, х86)
- Microsoft Windows 8 ( х64, х86)
- Microsoft Windows 10 (х64, х86)
### **линукс**
- Убунту
- OpenSUSE
- CentOS
- и другие

## Системные требования для целевой платформы Linux

- Библиотеки времени выполнения GCC-6 (или более поздней версии).

- Зависимости .NET Core Runtime. Установка самой .NET Core Runtime НЕ требуется.

- Для Python 3.5–3.7: требуется сборка `pymalloc` версии Python. Параметр сборки `--with-pymalloc` Python включен по умолчанию. Обычно сборка `pymalloc` Python помечается суффиксом `m` в имени файла.

- `libpython` общая библиотека Python. Опция сборки `--enable-shared` Python отключена по умолчанию, некоторые дистрибутивы Python не содержат разделяемой библиотеки `libpython`. Для некоторых платформ Linux общую библиотеку `libpython` можно установить с помощью диспетчера пакетов, например: `sudo apt-get install libpython3.7`. Распространенная проблема заключается в том, что библиотека `libpython` устанавливается не в стандартное системное расположение для общих библиотек. Проблема может быть устранена с помощью параметров сборки Python для установки альтернативных путей к библиотекам при компиляции Python или путем создания символической ссылки на файл библиотеки `libpython` в системном стандартном местоположении для общих библиотек. Обычно имя файла общей библиотеки `libpython` — `libpythonX.Ym.so.1.0` для Python 3.5-3.7 или `libpythonX.Y.so.1.0` для Python 3.8 или более поздней версии (например: libpython3.7m.so.1.0, libpython3.9.so.1.0).
