---
title: Validar archivos XBRL y iXBRL en Python
linktitle: Validar archivos XBRL y iXBRL
keywords: xbrl taxonomy,xbrl,ixbrl,xbrl linkbases,xbrl Instances
description: Python Finance La biblioteca API puede validar los archivos XBRL y iXBRL. Consulte los códigos de ejemplo proporcionados en este artículo para obtener más información.
type: docs
weight: 30
url: /es/python-net/validate-xbrl-and-ixbrl-files/
---
## **Valide el archivo de instancia XBRL en Python**
 Las instancias XBRL, las bases de enlaces XBRL y los esquemas de taxonomía XBRL DEBEN cumplir con los requisitos de sintaxis impuestos en[XBRL especificación](http://www.xbrl.org/Specification/XBRL-2.1/REC-2003-12-31/XBRL-2.1-REC-2003-12-31+corrected-errata-2013-02-20.html). Para validarlos, la clase XbrlInstance proporciona el método validate().

El siguiente fragmento de código Python muestra cómo validar un documento de instancia XBRL.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-xbrl-instance-file.py" >}}
## **Validar archivo iXBRL en Python**
 los[iXBRL especificación](http://www.xbrl.org/specification/inlinexbrl-part1/rec-2013-11-18/inlinexbrl-part1-rec-2013-11-18.html) define muchas reglas de validación. Para validar archivos iXBRL, la clase InlineXbrlDocument proporciona un método de validación().

El siguiente fragmento de código Python demuestra la validación de un documento de instancia iXBRL.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "validate-ixbrl-file.py" >}}
## **Códigos de error de validación**
 En la enumeración ValidationErrorCode, los códigos de error de validación se definen para cada regla de validación.
Las siguientes son las definiciones de los códigos de error:

- CONTEXTO_PERÍODO_NO_COMIENZO_HORA: el tipo de período de contexto es la duración, pero no tiene fecha de inicio.
- CONTEXTO_PERÍODO_NO_FINAL_TIME: el tipo de período de contexto es la duración, pero no tiene fecha de finalización.
- CONTEXTO_PERÍODO_COMIENZO_DESPUÉS_FIN: el tipo de período de contexto es la duración, pero la fecha de finalización es anterior a la fecha de inicio.
- CONTEXTO_INSTANTE_NO_TIME: el tipo de período de contexto es instantáneo, pero no tiene fecha instantánea.
- CONTEXTO_GUIÓN_XBRL_NAMESPACE: el escenario de contexto no puede tener el nodo de espacio de nombres XBRL.
- CONTEXTO_GUIÓN_XBRL_SUSTITUCIÓN_GRUPO: el escenario de contexto no puede tener un elemento en el grupo de sustitución de elementos definidos en el espacio de nombres XBRL.
- CONTEXTO_GUIÓN_VACÍO: el escenario de contexto no puede estar vacío.
- CONTEXTO_SEGMENTO_XBRL_NAMESPACE: el segmento de contexto no puede tener el nodo de espacio de nombres XBRL.
- CONTEXTO_SEGMENTO_XBRL_SUBSTITUTIONGROUP: el segmento de contexto no puede tener elementos en el grupo de sustitución para elementos definidos en el espacio de nombres XBRL.
- CONTEXTO_SEGMENTO_VACÍO: el segmento de contexto no puede estar vacío.
- ARTÍCULO_NO_CONTEXTO: El elemento debe tener un contexto.
- ARTÍCULO_PEROIDE_ESCRIBE_CONFLICTO_WITH_CONTEXT: el elemento tiene un conflicto de tipo de período con el contexto.
- ARTÍCULO_NUMÉRICO_NO_UNIT: El artículo es numérico y debe tener una unidad.
- MONETARIO_ARTÍCULO_NO_ÚNICO_UNIT_MEASURE: El artículo es de tipo monetario y debe tener una sola unidad de medida.
- MONETARIO_ARTÍCULO_NO_ISO4217: El artículo es de tipo monetario y debe tener una unidad de medida de estilo ISO 4217.
- CUOTA_ARTÍCULO_NO_ÚNICO_UNIT_MEASURE: el artículo es un tipo de recurso compartido y debe tener una sola unidad de medida.
- CUOTA_ARTÍCULO_NO_CUOTA_UNIT_MEASURE: El elemento es de tipo compartido y debe tener una unidad de medida xbrli:shares.
- NULO_ARTÍCULO_CON_PRECISIÓN_OR_DECIMALS: El artículo es nulo y no debe tener ni precisión ni decimales.
- FRACCIÓN_ARTÍCULO_CON_PRECISIÓN_OR_DECIMALS: El elemento es un tipo de fracción y no debe tener ni precisión ni decimales.
- NUMÉRICO_ARTÍCULO_CON_AMBAS COSAS_PRECISIÓN_Y_DECIMALES: El ítem es de tipo numérico y no debe tener tanto precisión como decimales.
- NUMÉRICO_ARTÍCULO_SIN QUE_PRECISIÓN_OR_DECIMALS: el elemento es de tipo numérico y debe tener precisión o decimales.
- NO_NUMÉRICO_ARTÍCULO_CON_PRECISIÓN_O_DECIMALES: El ítem no es de tipo numérico y no debe tener ni precisión ni decimales.
- NOTA_ARCO_DE_NO_ENCONTRADO: No se pudo encontrar el arco de la nota al pie de Loc.
- NOTA_ARCO_A_NO_ENCONTRADO: No se puede encontrar el arco de la nota al pie en la nota al pie.
- DEFINICIÓN_ARCO_DE_NO_ENCONTRADO: No se pudo encontrar el arco de Definición de Loc.
- DEFINICIÓN_ARCO_A_NO_ENCONTRADO: No se pudo encontrar el arco de definición a Loc.
- ESENCIA_ALIAS_DEFINICIÓN_ARCO_DIFFERENT_TYPE: El arco de definición de alias de esencia tiene diferentes tipos.
- ESENCIA_ALIAS_DEFINICIÓN_ARCO_DIFERENTE_PERÍODO_TIPO: El arco de definición de alias de esencia tiene diferentes tipos de períodos.
- ESENCIA_ALIAS_DEFINICIÓN_ARCO_DIFFERENT_BALANCE: El arco de definición de alias de esencia tiene diferentes saldos.
- CÁLCULO_ARCO_DE_NO_ENCONTRADO: No se puede encontrar el arco de cálculo de Loc.
- CÁLCULO_ARCO_A_NO_ENCONTRADO: No se pudo encontrar el arco de Cálculo a Loc.
- ETIQUETA_ARCO_DE_NO_ENCONTRADO: No se pudo encontrar el arco de Lable de Loc.
- ETIQUETA_ARCO_A_NO_ENCONTRADO: No se pudo encontrar el arco de Lable a Loc.
- PRESENTACIÓN_ARCO_DE_NO_ENCONTRADO: No se pudo encontrar un arco de presentación de Loc.
- PRESENTACIÓN_ARCO_A_NO_ENCONTRADO: No se pudo encontrar un arco de presentación para Loc.
- REFERENCIA_ARCO_DE_NO_ENCONTRADO: No se puede encontrar un arco de referencia de Loc.
- REFERENCIA_ARCO_A_NO_ENCONTRADO: No se pudo encontrar un arco de referencia a Loc.
### **Ejemplo de mensaje de error de validación estándar**
![todo:imagen_alternativa_texto](validate-xbrl-and-ixbrl-files_1.png)

Arriba hay una instancia XBRL, define el contexto "cd1", este tipo de período de contexto es duración, su fecha de inicio es 2002-03-31, la fecha de finalización es 2001-03-31, por lo que la fecha de finalización es anterior a la fecha de inicio. En la especificación XBRL, capítulo 4.7.2, define la regla de validación: "la fecha de finalización DEBE especificar o implicar un punto en el tiempo que es posterior al punto en el tiempo especificado o implícito de la correspondiente fecha de inicio". Según esta regla, esta instancia XBRL no es válida.
## **Valide XBRL y genere un mensaje de error estándar**
El siguiente código valida la instancia XBRL y genera el mensaje de error estándar.

{{< gist "aspose-finance-gists" "e1df624c58dc6f522a87f29ceb041dd9" "ValidateXBRLWithStardardErrorMessage.py" >}}

La siguiente imagen muestra la salida:

![todo:imagen_alternativa_texto](validate-xbrl-and-ixbrl-files_2.png)



