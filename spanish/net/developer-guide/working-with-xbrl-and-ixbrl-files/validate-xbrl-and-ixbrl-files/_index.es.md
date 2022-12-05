---
title: Validar archivos XBRL y iXBRL en C#
linktitle: Validar archivos XBRL y iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: C# Finance La biblioteca API puede validar los archivos XBRL y iXBRL. Consulte los códigos de ejemplo proporcionados en este artículo para obtener más información.
type: docs
weight: 30
url: /es/net/validate-xbrl-and-ixbrl-files/
---
## **Valide el archivo de instancia XBRL en C#**
 Las instancias XBRL, las bases de enlaces XBRL y los esquemas de taxonomía XBRL DEBEN cumplir con los requisitos de sintaxis impuestos en[XBRL especificación](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Para validar estos, el[XbrlInstancia](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance) la clase proporciona la[Validar()](https://reference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/methods/validate) método.

El siguiente fragmento de código C# muestra cómo validar un documento de instancia XBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXbrlInstance.cs" >}}
## **Validar archivo iXBRL en C#**
 los[iXBRL especificación](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html)define muchas reglas de validación. Para validar archivos iXBRL, el[InlineXbrlDocumentInlineXbrlDocument](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument) la clase proporciona un[Validar()](https://reference.aspose.com/finance/net/aspose.finance.xbrl.inline/inlinexbrldocument/methods/validate) método.

El siguiente fragmento de código C# demuestra la validación de un documento de instancia iXBRL.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateIxbrlInstance.cs" >}}
## **Códigos de error de validación**
 en la enumeración[Código de error de validación](https://reference.aspose.com/finance/net/aspose.finance.xbrl.validator/validationerrorcode) , los códigos de error de validación se definen para cada regla de validación.
Las siguientes son las definiciones de los códigos de error:

- ContextPeriodNoStartTime: el tipo de período de contexto es la duración, pero no tiene fecha de inicio.
- ContextPeriodNoEndTime: el tipo de período de contexto es la duración, pero no tiene fecha de finalización.
- ContextPeriodStartAfterEnd: el tipo de período de contexto es la duración, pero la fecha de finalización es anterior a la fecha de inicio.
- ContextInstantNoTime: el tipo de período de contexto es instantáneo, pero no tiene fecha instantánea.
- ContextScenarioXbrlNamespace: el escenario de contexto no puede tener el nodo de espacio de nombres XBRL.
- ContextScenarioXbrlSubstitutionGroup: el escenario de contexto no puede tener un elemento en el grupo de sustitución para elementos definidos en el espacio de nombres XBRL.
- ContextScenarioEmpty: el escenario de contexto no puede estar vacío.
- ContextSegmentXbrlNamespace: el segmento de contexto no puede tener el nodo de espacio de nombres XBRL.
- ContextSegmentXbrlSubstitutionGroup: el segmento de contexto no puede tener elementos en el grupo de sustitución para elementos definidos en el espacio de nombres XBRL.
- ContextSegmentEmpty: el segmento de contexto no puede estar vacío.
- ItemNoContext: el elemento debe tener un contexto.
- ItemPeroidTypeConflictWithContext: el elemento tiene un conflicto de tipo de período con el contexto.
- ItemNumericNoUnit: el artículo es numérico y debe tener una unidad.
- MonetaryItemNoSingleUnitMeasure: el artículo es de tipo monetario y debe tener una sola unidad de medida.
- MonetaryItemNoISO4217: el artículo es de tipo monetario y debe tener una unidad de medida de estilo ISO 4217.
- ShareItemNoSingleUnitMeasure: el artículo es un tipo de recurso compartido y debe tener una sola unidad de medida.
- ShareItemNoShareUnitMeasure: el elemento es de tipo compartido y debe tener una unidad de medida xbrli:shares.
- NillItemWithPrecisionOrDecimals: el elemento es nulo y no debe tener precisión ni decimales.
- FractionItemWithPrecisionOrDecimals: el elemento es un tipo de fracción y no debe tener precisión ni decimales.
- NumericItemWithBothPrecisionAndDecimals: el elemento es de tipo numérico y no debe tener precisión ni decimales.
- NumericItemWithoutPrecisionOrDecimals: el elemento es de tipo numérico y debe tener precisión o decimales.
- NonNumericItemWithPrecisionOrDecimals: el elemento no es de tipo numérico y no debe tener precisión ni decimales.
- FootnoteArcFromNotFound: no se puede encontrar el arco de la nota al pie de Loc.
- FootnoteArcToNotFound: no se puede encontrar el arco de la nota al pie en la nota al pie.
- DefinitionArcFromNotFound: no se puede encontrar el arco de definición de Loc.
- DefinitionArcToNotFound: no se puede encontrar el arco de definición para Loc.
- EssenceAliasDefinitionArcDifferentType: el arco de definición de alias de esencia tiene diferentes tipos.
- EssenceAliasDefinitionArcDifferentPeriodType: el arco de definición de alias de esencia tiene diferentes periodTypes.
- EssenceAliasDefinitionArcDifferentBalance: el arco de definición de alias de esencia tiene diferentes saldos.
- CalculationArcFromNotFound: no se puede encontrar el arco de cálculo de Loc.
- CalculationArcToNotFound: no se puede encontrar el arco de cálculo para Loc.
- LabelArcFromNotFound: no se puede encontrar el arco de etiqueta de Loc.
- LabelArcToNotFound: no se puede encontrar el arco de etiquetas en la ubicación.
- PresentationArcFromNotFound: no se puede encontrar un arco de presentación de Loc.
- PresentationArcToNotFound: no se puede encontrar un arco de presentación para Loc.
- ReferenceArcFromNotFound: no se puede encontrar un arco de referencia de Loc.
- ReferenceArcToNotFound: no se puede encontrar un arco de referencia para Loc.
### **Ejemplo de mensaje de error de validación estándar**
![todo:imagen_alternativa_texto](validate-xbrl-and-ixbrl-files_1.png)

Arriba hay una instancia XBRL, define el contexto "cd1", este tipo de período de contexto es duración, su fecha de inicio es 2002-03-31, la fecha de finalización es 2001-03-31, por lo que la fecha de finalización es anterior a la fecha de inicio. En la especificación XBRL, capítulo 4.7.2, define la regla de validación: "la fecha de finalización DEBE especificar o implicar un punto en el tiempo que es posterior al punto en el tiempo especificado o implícito de la correspondiente fecha de inicio". Según esta regla, esta instancia XBRL no es válida.
## **Valide XBRL y genere un mensaje de error estándar**
El siguiente código valida la instancia XBRL y genera el mensaje de error estándar.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithStardardErrorMessage.cs" >}}

La siguiente imagen muestra la salida:

![todo:imagen_alternativa_texto](validate-xbrl-and-ixbrl-files_2.png)
## **Valide XBRL y emita un mensaje de error personalizado**
El siguiente código valida la instancia XBRL y genera un mensaje de error personalizado.

{{< gist "aspose-com-gists" "d3d183d03a9cc8e4ce248a95919a6cff" "ValidateXBRLWithCustomizedErrorMessage.cs" >}}

La siguiente imagen muestra la salida:

![todo:imagen_alternativa_texto](validate-xbrl-and-ixbrl-files_3.png)

**Valide XBRL y genere un mensaje de error estándar**


