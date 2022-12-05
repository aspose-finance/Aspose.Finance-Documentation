---
title: Преобразование XBRL в iXBRL в C#
linktitle: Преобразовать XBRL в IXBRL
type: docs
weight: 10
url: /ru/net/convert-xbrl-to-ixbrl/
description: C# Finance Библиотека API поддерживает преобразование файлов XBRL в iXBRL. См. код, представленный в этой статье.
---
 Aspose.Finance поддерживает преобразование файлов XBRL в IXBRL путем передачи экземпляра[**СохранитьОпции**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/saveoptions) класс к[**XbrlDocument.Save**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save/index) метод. Чтобы сохранить документ в формате IXBRL, установите[**SaveOptions.SaveFormat**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/saveoptions/properties/saveformat) к[**СохранитьФормат.IXBRL**](https://reference.aspose.com/finance/net/aspose.finance.xbrl/saveformat).

В следующем фрагменте кода C# показано, как преобразовать XBRL в формат IXBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "CSharp-Conversion-ConvertXbrlToIXbrl-1.cs" >}}
