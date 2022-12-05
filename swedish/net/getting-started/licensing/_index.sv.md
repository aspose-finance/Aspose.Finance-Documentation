---
title: Licensiering
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /sv/net/licensing/
description: C# Finance Bibliotek API bjuder in sina kunder att skaffa en klassisk licens och mätlicens. Samt använda en begränsad licens för att bättre utforska produkten.
---
## **Värdera Aspose.Finance**
Du kan enkelt ladda ner Aspose.Finance for .NET produkt för utvärderingsändamål. Vänligen se[Aspose.Finance for .NET nedladdningssida](https://www.nuget.org/packages/Aspose.Finance/)för att ta reda på den senaste versionen. Utvärderingsversionen ger absolut samma möjligheter som den licensierade versionen av komponenten. Dessutom blir utvärderingsversionen helt enkelt licensierad när du lägger till några rader kod för att tillämpa licensen.

### **Begränsningar för utvärderingsversion**
Utvärderingsversionen innehåller alla funktioner utom följande:

- **Antal öppnade filer** (Aspose.Finance) När du kör ditt program kan du bara öppna 50 filer med Aspose.Finance-biblioteket. Om din ansökan överstiger detta antal kommer ett undantag att kastas.
- **Antal sparade filer** (Aspose.Finance) När du kör ditt program kan du bara öppna 50 filer med Aspose.Finance-biblioteket. Om din ansökan överstiger detta antal kommer ett undantag att kastas.

{{% alert color="primary" %}} 

 Om du vill prova Aspose.Finance utan utvärderingsbegränsningar, begär en 30 dagars tillfällig licens. Vänligen hänvisa till[Hur får man en tillfällig licens?](https://purchase.aspose.com/temporary-license) för mer information.

{{% /alert %}} 
## **Ansöker om en licens**
 När du är nöjd med din[utvärdering](https://downloads.aspose.com/finance/net) av Aspose.Finance for .NET, köp en licens på webbplatsen Aspose:[Köpportal](https://purchase.aspose.com/buy) Bekanta dig med de olika licenstyperna. Om du har några frågor,[kontakta Aspose säljteamet](https://about.aspose.com/contact) och de hjälper dig gärna.

Varje Aspose-licens innehåller en ettårsprenumeration för gratis uppgraderingar till alla nya versioner eller korrigeringar som kommer ut under denna tid. Vi tillhandahåller gratis och obegränsad teknisk support till både licensierade användare och utvärderingsanvändare.

Licensen är en XML-fil i vanlig text som innehåller detaljer som produktnamn, antal licensierade utvecklare, prenumerations utgångsdatum och så vidare. Filen är digitalt signerad, så ändra inte filen: även om du lägger till en extra radbrytning i filen blir den ogiltig.
### **När ska man ansöka om en licens**
Följ dessa enkla regler:

- Licensen behöver bara ställas in en gång per applikationsdomän.
- Du måste ställa in licensen innan du använder andra Aspose.Finance-klasser.
- Att anropa SetLicense flera gånger är inte skadligt, men slösar bort processortid.
- Om du utvecklar en Windows Forms eller konsolapplikation, ring SetLicense i startkoden innan du använder Aspose.Finance klasser.
- När du utvecklar en ASP.NET-applikation, anrop SetLicense från filen Global.asax.cs, i den skyddade metoden Aplication_Start. Den anropas en gång när applikationen startar.
- Anropa inte SetLicense från Page_Load-metoderna eftersom det betyder att licensen kommer att laddas varje gång en webbsida laddas.
- Om du utvecklar ett klassbibliotek anropar du SetLicense från en statisk konstruktor av klassen som använder Aspose.Finance. Den statiska konstruktorn körs innan en instans av din klass skapas och ser till att Aspose.Finance-licensen är korrekt inställd.
### **Tillämpa licens med File eller Stream Object**
 Använd[License.SetLicense](https://reference.aspose.com/finance/net/aspose.finance/license) metod för att licensiera komponenten. Det enklaste sättet att ställa in en licens är att lägga licensfilen i samma mapp som Aspose.Finance.dll och ange filnamnet, utan sökväg, som visas nedan.
#### **Laddar en licens från fil**
Det här kodavsnittet initierar en licens som lagras i en fil eller i en inbäddad resurs.

```csharp

public static void SetLicenseExample()
{
    // Initialize license object
    Aspose.Finance.License license = new Aspose.Finance.License();
    try
    {
        // Set license
        license.SetLicense("Aspose.Finance.lic");
    }
    catch (Exception)
    {
        // something went wrong
        throw;
    }
    Console.WriteLine("License set successfully.");
}
```
#### **Ladda en licens från ett strömobjekt**
Dessa kodavsnitt initierar licensen från stream.

```csharp
public static void SetLicenseFromStream()
{
    // Initialize license object
    Aspose.Finance.License license = new Aspose.Finance.License();
    // Load license from the file stream
    System.IO.FileStream myStream =
        new System.IO.FileStream(
            "Aspose.Finance.lic",
            System.IO.FileMode.Open);
    // Set license
    license.SetLicense(myStream);
    Console.WriteLine("License set successfully.");
}
```
## **Tillämpa mätlicens**
Aspose.Finance for .NET API tillåter utvecklare att tillämpa mätlicens. Det är en ny licensmekanism. Den nya licensmekanismen kommer att användas tillsammans med den befintliga licensmetoden. De kunder som vill bli fakturerade baserat på användningen av API-funktionerna kan använda den uppmätta licensen. För mer information, se[Metered Licensing FAQ](https://purchase.aspose.com/faqs/licensing/metered)sektion.

En ny klass[Uppmätt](https://reference.aspose.com/finance/net/aspose.finance/metered)har lagts till för att tillämpa mätt nyckel. Detta kodexempel visar hur man ställer in mätta offentliga och privata nycklar:

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
