---
title: Deklaration
type: docs
weight: 30
url: /sv/net/declaration/
---
## **Partiell Trust / Medium Trust Challenge**
Alla Aspose .NET komponenter kräver Full Trust-behörighetsuppsättningen. Anledningen är att Aspose .NET komponenter behöver komma åt registerinställningar, andra systemfiler än en virtuell katalog för vissa operationer som att tolka typsnitt, etc. Dessutom är Aspose .NET Komponenter baserade på kärnan .NET som kräver fullständiga systembehörigheter som även kräver fullständiga systembehörigheter. fall.

Internetleverantörer som är värd för flera applikationer från olika företag tillämpar oftast Medium Trust säkerhetsnivå. I fallet med .NET 2.0 tillämpar sådan säkerhetsnivå följande begränsningar:

- · **OleDbPermission** är inte tillgänglig. Det betyder att du inte kan använda den hanterade OLE DB-dataleverantören ADO.NET för att komma åt databaser.
- · **EventLogPermission** är inte tillgänglig. Det betyder att du inte kan komma åt händelseloggen Windows.
- · **ReflectionPermission** är inte tillgänglig. Det betyder att du inte kan använda reflektion.
- · **RegistryPermission** är inte tillgänglig. Det betyder att du inte kan komma åt registret.
- · **WebPermission** är begränsad. Detta innebär att din applikation endast kan kommunicera med en adress eller adressintervall som du definierar i<trust> element.
- · **FileIOPermission** är begränsad. Det betyder att du bara kan komma åt filer i din applikations virtuella kataloghierarki.

På grund av de skäl som anges ovan kan komponenterna Aspose .NET inte användas på servrar som ger andra behörighetsuppsättningar än Full Trust.
