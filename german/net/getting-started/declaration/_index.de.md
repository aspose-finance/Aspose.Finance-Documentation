---
title: Erklärung
type: docs
weight: 30
url: /de/net/declaration/
---
## **Teilweise Vertrauenswürdigkeit/mittlere Vertrauensherausforderung**
Alle Aspose .NET-Komponenten erfordern den Berechtigungssatz „Full Trust“. Der Grund dafür ist, dass Aspose .NET-Komponenten auf Registrierungseinstellungen und andere Systemdateien als ein virtuelles Verzeichnis für bestimmte Vorgänge wie das Analysieren von Schriftarten usw. zugreifen müssen. Darüber hinaus basieren Aspose .NET-Komponenten auf .NET-Kernsystemklassen, für die in vielen Fällen auch die Berechtigung „Full Trust“ erforderlich ist Fälle.

Internetdienstanbieter, die mehrere Anwendungen von verschiedenen Unternehmen hosten, erzwingen meist die Sicherheitsstufe „Medium Trust“. Im Fall von .NET 2.0 gelten für diese Sicherheitsstufe die folgenden Einschränkungen:

- · **OleDbPermission** ist nicht verfügbar. Das bedeutet, dass Sie den verwalteten OLE DB-Datenanbieter ADO.NET nicht für den Zugriff auf Datenbanken verwenden können.
- · **EventLogPermission** ist nicht verfügbar. Das bedeutet, dass Sie nicht auf das Ereignisprotokoll Windows zugreifen können.
- · **ReflectionPermission** ist nicht verfügbar. Dies bedeutet, dass Sie keine Reflexion verwenden können.
- · **RegistryPermission** ist nicht verfügbar. Dies bedeutet, dass Sie nicht auf die Registrierung zugreifen können.
- · **WebPermission** ist eingeschränkt. Das bedeutet, dass Ihre Anwendung nur mit einer Adresse oder einem Adressbereich kommunizieren kann, die Sie in der definieren<trust> Element.
- · **FileIOPermission** ist eingeschränkt. Das bedeutet, dass Sie nur auf Dateien in der virtuellen Verzeichnishierarchie Ihrer Anwendung zugreifen können.

Aus den oben genannten Gründen können Aspose .NET-Komponenten nicht auf Servern verwendet werden, die einen anderen Berechtigungssatz als Volles Vertrauen gewähren.
