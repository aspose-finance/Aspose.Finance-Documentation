---
title: متطلبات النظام
second_title: Aspose.Finance for Python via .NET
type: docs
weight: 50
url: /ar/python-net/system-requirements/
description:  تعرف على متطلبات النظام لـ Python Finance Library API
---
## **أنظمة التشغيل المدعومة**
### **Windows**
- Microsoft Windows 2000 (x64، x86)
- Microsoft Windows XP (x64، x86)
- Microsoft Windows Server 2003 (x64، x86)
- Microsoft Windows Server 2008 (x64، x86)
- Microsoft Windows Server 2012 (x64، x86)
- Microsoft Windows Vista (x64، x86)
- Microsoft Windows 7 (x64، x86)
- Microsoft Windows 8 (x64، x86)
- Microsoft Windows 10 (x64، x86)
### **لينكس**
- أوبونتو
- OpenSUSE
- CentOS
- و اخرين

## متطلبات النظام لمنصة لينكس الهدف

- مكتبات وقت تشغيل GCC-6 (أو أحدث).

- تبعيات .NET Core Runtime. تثبيت .NET Core Runtime نفسه غير مطلوب.

- بالنسبة إلى Python 3.5-3.7: يلزم إنشاء `pymalloc` من Python. يتم تمكين خيار البناء `--with-pymalloc` Python افتراضيًا. عادةً ما يتم تمييز `pymalloc` إنشاء Python بلاحقة `m` في اسم الملف.

- `libpython` شارك Python مكتبة. يتم تعطيل خيار الإنشاء `--enable-shared` Python افتراضيًا ، ولا تحتوي بعض توزيعات Python على المكتبة المشتركة `libpython`. بالنسبة لبعض أنظمة التشغيل Linux ، يمكن تثبيت المكتبة المشتركة `libpython` باستخدام مدير الحزم ، على سبيل المثال: `sudo apt-get install libpython3.7`. المشكلة الشائعة هي أن مكتبة `libpython` مثبتة في موقع مختلف عن موقع النظام القياسي للمكتبات المشتركة. يمكن إصلاح المشكلة باستخدام خيارات إنشاء Python لتعيين مسارات مكتبة بديلة عند تجميع Python ، أو إصلاحها عن طريق إنشاء ارتباط رمزي لملف مكتبة `libpython` في الموقع القياسي للنظام للمكتبات المشتركة. عادةً ما يكون اسم ملف المكتبة المشتركة `libpython` هو `libpythonX.Ym.so.1.0` لـ Python 3.5-3.7 ، أو `libpythonX.Y.so.1.0` لـ Python 3.8 أو أحدث (على سبيل المثال: libpython3.7m.so.1.0 ، libpython3.9.so.1.0).
