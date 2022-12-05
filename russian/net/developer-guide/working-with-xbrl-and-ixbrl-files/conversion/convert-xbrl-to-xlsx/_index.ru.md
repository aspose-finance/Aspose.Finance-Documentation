---
title: Преобразование XBRL в Excel XLSX в C#
linktitle: Конвертировать XBRL в XLSX
type: docs
weight: 10
url: /ru/net/convert-xbrl-to-xlsx/
description: C# Finance Библиотека API поддерживает преобразование файлов XBRL в Excel XLSX. Пожалуйста, ознакомьтесь с кодом, представленным в этой статье.
---
 Aspose.Finance поддерживает преобразование файлов XBRL в XLSX путем передачи экземпляра[**СохранитьОпции**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/saveoptions) класс к[**XbrlDocument.Save**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save/index) метод. Чтобы сохранить документ в формате XLSX, установите[**SaveOptions.SaveFormat**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/saveoptions/properties/saveformat) к[**СохранитьФормат.XLSX**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/saveformat).

В следующем фрагменте кода C# показано, как преобразовать XBRL в XLSX.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "CSharp-Conversion-ConvertXbrlToXlsx-1.cs" >}}
