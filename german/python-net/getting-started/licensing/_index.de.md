---
title: Lizenzierung
second_title: Aspose.Finance for .NET
type: docs
weight: 50
url: /de/python-net/licensing/
description: Python Finance Die Bibliothek API lädt ihre Kunden ein, eine Classic-Lizenz und eine Metered-Lizenz zu erwerben. Verwenden Sie außerdem eine eingeschränkte Lizenz, um das Produkt besser zu erkunden.
---
Manchmal möchten Sie, um das System besser zu studieren, so schnell wie möglich in den Code eintauchen. Um dies zu vereinfachen, bietet Aspose.Finance verschiedene Pläne zum Kauf an oder bietet eine kostenlose Testversion und eine 30-tägige temporäre Lizenz zur Evaluierung an.

{{% alert color="primary" %}}

 Beachten Sie, dass es eine Reihe allgemeiner Richtlinien und Praktiken gibt, die Sie bei der Bewertung, ordnungsgemäßen Lizenzierung und dem Kauf unserer Produkte anleiten. Sie finden sie im["Kaufrichtlinien und FAQ"](https://purchase.aspose.com/policies) Sektion.

{{% /alert %}}

## **Aspose.Finance auswerten**
 Sie können Aspose.Finance zur Evaluierung einfach herunterladen. Das Evaluierungspaket ist das gleiche wie das gekaufte Paket. Die Evaluierungsversion wird einfach lizenziert, nachdem Sie einige Codezeilen hinzugefügt haben, um die Lizenz anzuwenden.

### **Einschränkungen der Evaluierungsversion**
Die Evaluierungsversion bietet alle Funktionen mit Ausnahme der folgenden:

- **Anzahl der geöffneten Dateien** (Aspose.Finance) Wenn Sie Ihr Programm ausführen, können Sie nur 50 Dateien mit der Bibliothek Aspose.Finance öffnen. Wenn Ihre Anwendung diese Zahl überschreitet, wird eine Ausnahme ausgelöst.
- **Anzahl gespeicherter Dateien** (Aspose.Finance) Wenn Sie Ihr Programm ausführen, können Sie nur 50 Dateien mit der Bibliothek Aspose.Finance öffnen. Wenn Ihre Anwendung diese Zahl überschreitet, wird eine Ausnahme ausgelöst.

{{% alert color="primary" %}} 

 Wenn Sie Aspose.Finance ohne Evaluierungseinschränkungen ausprobieren möchten, fordern Sie eine temporäre 30-Tage-Lizenz an. Bitte beziehen Sie sich auf[Wie erhalte ich eine temporäre Lizenz?](https://purchase.aspose.com/temporary-license) für mehr Informationen.

{{% /alert %}} 

## **Über die Lizenz**
 Sie können ganz einfach eine Testversion von Aspose.Finance für Python über .NET herunterladen[Download-Seite](https://pypi.org/project/aspose.finance/) . Die Evaluierungsversion bietet absolut**die gleichen Fähigkeiten**als lizenzierte Version von Aspose.Finance. Darüber hinaus wird die Testversion einfach lizenziert, nachdem Sie eine Lizenz erworben und ein paar Codezeilen hinzugefügt haben, um die Lizenz anzuwenden.

Die Lizenz ist eine reine Text-XML-Datei, die Details wie den Produktnamen, die Anzahl der lizenzierten Entwickler, das Ablaufdatum des Abonnements usw. enthält. Die Datei ist digital signiert, ändern Sie die Datei also nicht. Selbst ein versehentliches Hinzufügen eines zusätzlichen Zeilenumbruchs zum Inhalt der Datei macht sie ungültig.

 Um die mit der Evaluierungsversion verbundenen Einschränkungen zu vermeiden, müssen Sie vor der Verwendung eine Lizenz festlegen**Aspose.Finance**. Sie müssen nur einmal pro Anwendung oder Prozess eine Lizenz festlegen.

## Gekaufte Lizenz

Nach dem Kauf müssen Sie die Lizenzdatei oder den Stream anwenden. Dieser Abschnitt beschreibt Möglichkeiten, wie dies geschehen kann, und kommentiert außerdem einige häufig gestellte Fragen.

{{% alert color="primary" %}}

Sie müssen die Lizenz festlegen:
* nur einmal pro Anwendungsdomäne
* bevor Sie andere Aspose.Finance-Klassen verwenden

{{% /alert %}}

{{% alert color="primary" %}}

Preisinformationen finden Sie auf der["Preisinformationen"](https://purchase.aspose.com/pricing/finance/family) Seite.

{{% /alert %}}

### **Festlegen einer Lizenz in Aspose.Finance für Python über .NET**

Lizenzen können von verschiedenen Orten aus beantragt werden:

* Explizite Pfad
* Der Ordner, der das Python-Skript enthält, das Aspose.Finance für Python über .NET aufruft
* Streamen
* Als Metered License – ein neuer Lizenzierungsmechanismus

{{% alert color="primary" %}}

 Verwenden Sie die**set_license** Methode zum Lizenzieren einer Komponente.

 Berufung**set_license** mehrmals ist nicht schädlich, es verschwendet nur Prozessorzeit.

{{% /alert %}}

 In den folgenden Abschnitten beschreiben wir die beiden gängigen Methoden zum Festlegen der Lizenz.

#### **Anwenden einer Lizenz mithilfe einer Datei**
Die einfachste Methode zum Festlegen einer Lizenz erfordert, dass Sie die Lizenzdatei in demselben Ordner ablegen, der das Python-Skript enthält, das Aspose.Finance für Python aufruft, und nur den Dateinamen ohne Pfad angeben.

Dieses Code-Snippet wird verwendet, um eine Lizenzdatei festzulegen:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license("Aspose.Finance.lic")
```

Beim Aufrufen der set_license-Methode sollte der Lizenzname mit dem Ihrer Lizenzdatei identisch sein. Beispielsweise können Sie den Namen der Lizenzdatei in „Aspose.Finance.lic.xml“ ändern. Dann müssen Sie in Ihrem Code den neuen Lizenznamen (Aspose.Finance.lic.xml) an die SetLicense-Methode übergeben.

#### **Anwenden einer Lizenz aus einem Stream**
 Sie können eine Lizenz aus einem Stream laden.

Dieses Code-Snippet wird verwendet, um eine Lizenz von einem Stream anzuwenden:

**Python**

```py
import aspose.finance as af

# Instantiate an instance of license and set the license file through its path
license = af.License()
license.set_license(stream)
```

#### Wenden Sie eine gemessene Lizenz an

Aspose.Finance ermöglicht es Entwicklern, einen gemessenen Schlüssel anzuwenden. Dies ist ein neuer Lizenzierungsmechanismus.

Der neue Lizenzierungsmechanismus wird zusammen mit der bestehenden Lizenzierungsmethode verwendet. Diejenigen Kunden, die basierend auf der Nutzung von API-Funktionen abgerechnet werden möchten, können die Metered Licensing verwenden.

 Nachdem Sie alle notwendigen Schritte abgeschlossen haben, um diesen Lizenztyp zu erhalten, erhalten Sie die Schlüssel, nicht die Lizenzdatei. Dieser gemessene Schlüssel kann mit angewendet werden**Gemessen** Klasse, die speziell für diesen Zweck eingeführt wurde.

Das folgende Codebeispiel zeigt, wie getaktete öffentliche und private Schlüssel festgelegt werden:

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

 Bitte beachten Sie, dass Sie für die korrekte Nutzung der Metered-Lizenz über eine stabile Internetverbindung verfügen müssen, da der Metered-Mechanismus für korrekte Berechnungen die ständige Interaktion mit unseren Diensten erfordert. Weitere Einzelheiten finden Sie unter[„FAQ zur getakteten Lizenzierung“](https://purchase.aspose.com/faqs/licensing/metered) Sektion.

{{% /alert %}}
