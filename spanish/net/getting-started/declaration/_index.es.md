---
title: Declaración
type: docs
weight: 30
url: /es/net/declaration/
---
## **Reto de confianza parcial/confianza media**
Todos los componentes Aspose .NET requieren el conjunto de permisos Plena confianza. La razón es que los componentes Aspose .NET necesitan acceder a la configuración del registro, archivos del sistema que no sean un directorio virtual para ciertas operaciones como analizar fuentes, etc. casos.

Los proveedores de servicios de Internet que alojan múltiples aplicaciones de diferentes compañías en su mayoría imponen un nivel de seguridad de confianza medio. En el caso de .NET 2.0, dicho nivel de seguridad aplica las siguientes restricciones:

- · **OleDbPermiso** no está disponible. Esto significa que no puede usar el proveedor de datos OLE DB administrado ADO.NET para acceder a las bases de datos.
- · **Permiso de registro de eventos** no está disponible. Esto significa que no puede acceder al registro de eventos Windows.
- · **ReflexiónPermiso** no está disponible. Esto significa que no puede usar la reflexión.
- · **RegistroPermiso** no está disponible. Esto significa que no puede acceder al registro.
- · **Permiso web** está restringido. Esto significa que su aplicación solo puede comunicarse con una dirección o rango de direcciones que usted defina en el<trust> elemento.
- · **ArchivoIOPermiso** está restringido. Esto significa que solo puede acceder a archivos en la jerarquía de directorios virtuales de su aplicación.

Debido a los motivos especificados anteriormente, los componentes Aspose .NET no se pueden usar en servidores que otorgan un conjunto de permisos que no sea Plena confianza.
