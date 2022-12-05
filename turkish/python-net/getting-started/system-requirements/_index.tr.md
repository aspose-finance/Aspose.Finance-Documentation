---
title: sistem gereksinimleri
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /tr/python-net/system-requirements/
description:  Python Finance Kütüphane API Sistem Gereksinimleri hakkında bilgi edinin
---
## **Desteklenen İşletim Sistemleri**
### **Windows**
- Microsoft Windows 2000 (x64, x86)
- Microsoft Windows XP ( x64, x86)
- Microsoft Windows Sunucu 2003 ( x64, x86)
- Microsoft Windows Sunucu 2008 ( x64, x86)
- Microsoft Windows Sunucu 2012 ( x64, x86)
- Microsoft Windows Vista ( x64, x86)
- Microsoft Windows 7 ( x64, x86)
- Microsoft Windows 8 ( x64, x86)
- Microsoft Windows 10 ( x64, x86)
### **linux**
- ubuntu
- OpenSUSE
- CentOS
- ve diğerleri

## Hedef Linux Platformu için Sistem Gereksinimleri

- GCC-6 çalışma zamanı kitaplıkları (veya üstü).

- .NET Core Runtime bağımlılıkları. .NET Core Runtime'ın kendisinin yüklenmesi gerekli DEĞİLDİR.

- Python 3.5-3.7 için: Python'in `pymalloc` yapısı gereklidir. `--with-pymalloc` Python oluşturma seçeneği varsayılan olarak etkindir. Tipik olarak, Python'in `pymalloc` yapısı, dosya adında `m` son ekiyle işaretlenir.

- `libpython` paylaşılan Python kitaplığı. `--enable-shared` Python oluşturma seçeneği varsayılan olarak devre dışıdır, bazı Python dağıtımları `libpython` paylaşılan kitaplığını içermez. Bazı linux platformları için, `libpython` paylaşımlı kitaplık, paket yöneticisi kullanılarak kurulabilir, örneğin: `sudo apt-get install libpython3.7`. Yaygın sorun, `libpython` kitaplığının, paylaşılan kitaplıklar için standart sistem konumundan farklı bir konuma yüklenmesidir. Sorun, Python derlenirken alternatif kitaplık yolları ayarlamak için Python oluşturma seçenekleri kullanılarak giderilebilir veya paylaşılan kitaplıklar için sistem standart konumunda `libpython` kitaplık dosyasına sembolik bir bağlantı oluşturarak giderilebilir. `libpython` paylaşılan kitaplık dosya adı genellikle Python 3.5-3.7 için `libpythonX.Ym.so.1.0` veya Python 3.8 veya sonrası için `libpythonX.Y.so.1.0`'dir (örneğin: libpython3.7m.so.1.0, libpython3.9.so.1.0).
