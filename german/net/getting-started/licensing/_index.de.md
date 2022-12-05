---
title: Lizenzierung
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /de/net/licensing/
description: C# Finance Die Bibliothek API lädt ihre Kunden ein, eine Classic-Lizenz und eine Metered-Lizenz zu erwerben. Verwenden Sie außerdem eine eingeschränkte Lizenz, um das Produkt besser zu erkunden.
---
## **Aspose.Finance auswerten**
Sie können das Produkt Aspose.Finance for .NET einfach zu Testzwecken herunterladen. Bitte wende dich an die[Aspose.Finance for .NET Download-Seite](https://www.nuget.org/packages/Aspose.Finance/)um die neuste Version herauszufinden. Die Evaluierungsversion bietet absolut dieselben Funktionen wie die lizenzierte Version der Komponente. Darüber hinaus wird die Evaluierungsversion einfach lizenziert, wenn Sie einige Codezeilen hinzufügen, um die Lizenz anzuwenden.

### **Einschränkungen der Evaluierungsversion**
Die Evaluierungsversion bietet alle Funktionen mit Ausnahme der folgenden:

- **Anzahl der geöffneten Dateien** (Aspose.Finance) Wenn Sie Ihr Programm ausführen, können Sie nur 50 Dateien mit der Bibliothek Aspose.Finance öffnen. Wenn Ihre Anwendung diese Zahl überschreitet, wird eine Ausnahme ausgelöst.
- **Anzahl gespeicherter Dateien** (Aspose.Finance) Wenn Sie Ihr Programm ausführen, können Sie nur 50 Dateien mit der Bibliothek Aspose.Finance öffnen. Wenn Ihre Anwendung diese Zahl überschreitet, wird eine Ausnahme ausgelöst.

{{% alert color="primary" %}} 

 Wenn Sie Aspose.Finance ohne Evaluierungseinschränkungen ausprobieren möchten, fordern Sie eine temporäre 30-Tage-Lizenz an. Bitte beziehen Sie sich auf[Wie erhalte ich eine temporäre Lizenz?](https://purchase.aspose.com/temporary-license) für mehr Informationen.

{{% /alert %}} 
## **Anwenden einer Lizenz**
 Sobald Sie mit Ihrem zufrieden sind[Auswertung](https://downloads.aspose.com/finance/net) von Aspose.Finance for .NET, kaufen Sie eine Lizenz auf der Aspose-Website:[Einkaufsportal](https://purchase.aspose.com/buy) Machen Sie sich mit den verschiedenen verfügbaren Lizenztypen vertraut. Wenn Sie irgendwelche Fragen haben,[Wenden Sie sich an das Verkaufsteam unter Aspose](https://about.aspose.com/contact) und sie helfen Ihnen gerne weiter.

Jede Aspose-Lizenz enthält ein einjähriges Abonnement für kostenlose Upgrades auf alle neuen Versionen oder Fixes, die während dieser Zeit herauskommen. Wir bieten sowohl lizenzierten als auch Evaluierungsbenutzern kostenlosen und unbegrenzten technischen Support.

Die Lizenz ist eine reine Text-XML-Datei, die Details wie den Produktnamen, die Anzahl der lizenzierten Entwickler, das Ablaufdatum des Abonnements usw. enthält. Die Datei ist digital signiert, ändern Sie die Datei also nicht: Selbst das Hinzufügen eines zusätzlichen Zeilenumbruchs zur Datei macht sie ungültig.
### **Wann eine Lizenz beantragt werden sollte**
Befolgen Sie diese einfachen Regeln:

- Die Lizenz muss nur einmal pro Anwendungsdomäne festgelegt werden.
- Sie müssen die Lizenz festlegen, bevor Sie andere Aspose.Finance-Klassen verwenden.
- Das mehrmalige Aufrufen von SetLicense schadet nicht, verschwendet aber Prozessorzeit.
- Wenn Sie eine Windows Forms- oder Konsolenanwendung entwickeln, rufen Sie SetLicense im Startcode auf, bevor Sie Aspose.Finance-Klassen verwenden.
- Rufen Sie beim Entwickeln einer ASP.NET-Anwendung SetLicense aus der Datei Global.asax.cs in der geschützten Methode Aplication_Start auf. Es wird einmal aufgerufen, wenn die Anwendung gestartet wird.
- Rufen Sie SetLicense nicht innerhalb der Page_Load-Methoden auf, da dies bedeutet, dass die Lizenz jedes Mal geladen wird, wenn eine Webseite geladen wird.
- Wenn Sie eine Klassenbibliothek entwickeln, rufen Sie SetLicense von einem statischen Konstruktor der Klasse auf, die Aspose.Finance verwendet. Der statische Konstruktor wird ausgeführt, bevor eine Instanz Ihrer Klasse erstellt wird, und stellt sicher, dass die Aspose.Finance-Lizenz richtig festgelegt ist.
### **Wenden Sie die Lizenz mit dem Datei- oder Stream-Objekt an**
 Verwenden Sie die[Lizenz.SetLicense](https://reference.aspose.com/finance/net/aspose.finance/license) Methode zum Lizenzieren der Komponente. Der einfachste Weg, eine Lizenz festzulegen, besteht darin, die Lizenzdatei in denselben Ordner wie die Aspose.Finance.dll zu legen und den Dateinamen ohne Pfad anzugeben, wie unten gezeigt.
#### **Laden einer Lizenz aus einer Datei**
Dieses Code-Snippet initialisiert eine Lizenz, die in einer Datei oder in einer eingebetteten Ressource gespeichert ist.

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
#### **Laden einer Lizenz aus einem Stream-Objekt**
Diese Codeausschnitte initialisieren die Lizenz aus dem Stream.

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
## **Wenden Sie eine gemessene Lizenz an**
Aspose.Finance for .NET API ermöglicht es Entwicklern, eine gemessene Lizenz anzuwenden. Es ist ein neuer Lizenzierungsmechanismus. Der neue Lizenzierungsmechanismus wird zusammen mit der bestehenden Lizenzierungsmethode verwendet. Diejenigen Kunden, die basierend auf der Nutzung der API-Funktionen abgerechnet werden möchten, können die gebührenpflichtige Lizenzierung verwenden. Weitere Einzelheiten finden Sie unter[Häufig gestellte Fragen zur getakteten Lizenzierung](https://purchase.aspose.com/faqs/licensing/metered)Sektion.

Eine neue Klasse[Gemessen](https://reference.aspose.com/finance/net/aspose.finance/metered)wurde hinzugefügt, um einen gemessenen Schlüssel anzuwenden. Dieses Codebeispiel zeigt, wie gemessene öffentliche und private Schlüssel festgelegt werden:

```csharp
public static void SetMeteredLicense()
{
    // Initialize a Metered license class object
    Aspose.Finance.Metered metered = new Aspose.Finance.Metered();
    // Apply public and private keys
    metered.SetMeteredKey("your-public-key", "your-private-key");
}
```
