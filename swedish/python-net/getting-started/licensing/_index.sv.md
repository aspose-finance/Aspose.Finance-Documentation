---
title: Licensiering
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /sv/python-net/licensing/
description: Python Finance Bibliotek API bjuder in sina kunder att skaffa en klassisk licens och mätlicens. Samt använda en begränsad licens för att bättre utforska produkten.
---
Ibland, för att studera systemet bättre, vill man dyka in i koden så snabbt som möjligt. För att göra detta enklare tillhandahåller Aspose.Finance olika planer för köp eller erbjuder en gratis provperiod och en 30-dagars tillfällig licens för utvärdering.

{{% alert color="primary" %}}

 Observera att det finns ett antal allmänna policyer och rutiner som vägleder dig om hur du utvärderar, licensierar och köper våra produkter. Du hittar dem i["Köppolicy och vanliga frågor"](https://purchase.aspose.com/policies) sektion.

{{% /alert %}}

## **Värdera Aspose.Finance**
 Du kan enkelt ladda ner Aspose.Finance för utvärdering. Utvärderingspaketet är detsamma som det köpta paketet. Utvärderingsversionen blir helt enkelt licensierad efter att du lagt till några rader kod för att tillämpa licensen.

### **Begränsningar för utvärderingsversion**
Utvärderingsversionen innehåller alla funktioner utom följande:

- **Antal öppnade filer** (Aspose.Finance) När du kör ditt program kan du bara öppna 50 filer med Aspose.Finance-biblioteket. Om din ansökan överstiger detta antal kommer ett undantag att kastas.
- **Antal sparade filer** (Aspose.Finance) När du kör ditt program kan du bara öppna 50 filer med Aspose.Finance-biblioteket. Om din ansökan överstiger detta antal kommer ett undantag att kastas.

{{% alert color="primary" %}} 

 Om du vill prova Aspose.Finance utan utvärderingsbegränsningar, begär en 30 dagars tillfällig licens. Vänligen hänvisa till[Hur får man en tillfällig licens?](https://purchase.aspose.com/temporary-license) för mer information.

{{% /alert %}} 

## **Om licensen**
 Du kan enkelt ladda ner en utvärderingsversion av Aspose.Finance för Python via .NET från dess[nedladdningssida](https://pypi.org/project/aspose.finance/) . Utvärderingsversionen ger absolut**samma förmågor**som den licensierade versionen av Aspose.Finance. Dessutom blir utvärderingsversionen helt enkelt licensierad efter att du köpt en licens och lägger till ett par rader kod för att tillämpa licensen.

Licensen är en XML-fil i vanlig text som innehåller information som produktnamn, antal utvecklare som den är licensierad till, prenumerationens utgångsdatum och så vidare. Filen är digitalt signerad, så ändra inte filen. Även ett oavsiktligt tillägg av en extra radbrytning till innehållet i filen kommer att ogiltigförklara den.

 För att undvika begränsningarna förknippade med utvärderingsversionen måste du ställa in en licens innan du använder den**Aspose.Finance**. Du behöver bara ange en licens en gång per ansökan eller process.

## Köpt licens

Efter köpet måste du tillämpa licensfilen eller streamen. Det här avsnittet beskriver alternativ för hur detta kan göras, och kommenterar även några vanliga frågor.

{{% alert color="primary" %}}

Du måste ställa in licensen:
* endast en gång per applikationsdomän
* innan du använder några andra Aspose.Finance-klasser

{{% /alert %}}

{{% alert color="primary" %}}

Du kan hitta prisinformation på["Prisinformation"](https://purchase.aspose.com/pricing/finance/family) sida.

{{% /alert %}}

### **Ange en licens i Aspose.Finance för Python via .NET**

Licenser kan tillämpas från olika platser:

* Explicit väg
* Mappen som innehåller pythonskriptet som anropar Aspose.Finance för Python via .NET
* Ström
* As a Metered License – en ny licensmekanism

{{% alert color="primary" %}}

 Använd**set_license** metod för att licensiera en komponent.

 Kallelse**set_license** flera gånger är inte skadligt, det slösar bara bort processortid.

{{% /alert %}}

 I avsnitten nedan kommer vi att beskriva de två vanliga metoderna som används för att ställa in licensen.

#### **Använda en licens med en fil**
Den enklaste metoden för att ställa in en licens kräver att du placerar licensfilen i samma mapp som innehåller python-skriptet som anropar Aspose.Finance för Python och anger bara filnamnet utan dess sökväg.

Detta kodavsnitt används för att ställa in en licensfil:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

När du anropar metoden set_license bör licensnamnet vara detsamma som för din licensfil. Du kan till exempel ändra licensfilens namn till "Aspose.Finance.lic.xml". Sedan, i din kod, måste du skicka det nya licensnamnet (Aspose.Finance.lic.xml) till SetLicense-metoden.

#### **Tillämpa en licens från en ström**
 Du kan ladda en licens från en stream.

Det här kodavsnittet används för att tillämpa en licens från en stream:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Tillämpa mätlicens

Aspose.Finance tillåter utvecklare att använda en mätnyckel. Detta är en ny licensmekanism.

Den nya licensmekanismen kommer att användas tillsammans med den befintliga licensmetoden. De kunder som vill bli fakturerade baserat på användningen av API-funktionerna kan använda Metered Licensing.

 När du har slutfört alla nödvändiga steg för att få den här typen av licens kommer du att få nycklarna, inte licensfilen. Denna mätnyckel kan appliceras med hjälp av**Uppmätt** klass speciellt införd för detta ändamål.

Följande kodexempel visar hur man ställer in mätta offentliga och privata nycklar:

```py
import aspose.finance as af

# Create an instance of CAD Metered class
metered = af.Metered()

# Access the set_metered_key property and pass public and private keys as parameters
metered.set_metered_key("*****", "*****")

# Get metered data amount before calling API
amountbefore = metered.get_consumption_quantity()
# Display information
print("Amount Consumed Before: " + str(amountbefore))

# handle finance file
# ......

# Get metered data amount After calling API
amountafter = metered.get_consumption_quantity()
# Display information
print("Amount Consumed After: " + str(amountafter))
```

{{% alert color="primary" %}}

 Observera att du måste ha en stabil Internetanslutning för korrekt användning av Metered-licensen, eftersom Metered-mekanismen kräver konstant interaktion med våra tjänster för korrekta beräkningar. För mer information, se["Vanliga frågor om mätning av licenser"](https://purchase.aspose.com/faqs/licensing/metered) sektion.

{{% /alert %}}
