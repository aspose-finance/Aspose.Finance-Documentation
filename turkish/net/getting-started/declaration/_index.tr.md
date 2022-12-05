---
title: beyanname
type: docs
weight: 30
url: /tr/net/declaration/
---
## **Kısmi Güven / Orta Güven Zorluğu**
Tüm Aspose .NET bileşenleri, Tam Güven izin seti gerektirir. Bunun nedeni, Aspose .NET bileşenlerinin, yazı tiplerini ayrıştırma gibi belirli işlemler için sanal dizin dışındaki sistem dosyalarına ve kayıt defteri ayarlarına erişmesi gerektiğidir. vakalar.

Farklı şirketlerden birden fazla uygulamayı barındıran İnternet Servis Sağlayıcıları, çoğunlukla Orta Güven güvenlik seviyesini zorunlu kılar. .NET 2.0 durumunda, bu güvenlik seviyesi aşağıdaki kısıtlamaları uygular:

- · **OleDbİzin** mevcut değil. Bu, veritabanlarına erişmek için ADO.NET tarafından yönetilen OLE DB veri sağlayıcısını kullanamayacağınız anlamına gelir.
- · **EventLogPermission** mevcut değil. Bu, Windows olay günlüğüne erişemeyeceğiniz anlamına gelir.
- · **Yansıma İzni** mevcut değil. Bu, yansımayı kullanamayacağınız anlamına gelir.
- · **Kayıt İzni** mevcut değil. Bu, kayıt defterine erişemeyeceğiniz anlamına gelir.
- · **Web İzni** kısıtlıdır. Bu, uygulamanızın yalnızca, içinde tanımladığınız bir adres veya adres aralığıyla iletişim kurabileceği anlamına gelir.<trust> eleman.
- · **Dosya IOPermission** kısıtlıdır. Bu, yalnızca uygulamanızın sanal dizin hiyerarşisindeki dosyalara erişebileceğiniz anlamına gelir.

Yukarıda belirtilen sebeplerden dolayı Aspose .NET bileşenleri Full Trust dışında izin seti veren sunucularda kullanılamaz.
