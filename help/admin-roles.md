---
title: Funciones de administrador
description: Con Adobe Admin Console, las organizaciones pueden definir una jerarquía administrativa flexible que permita una administración precisa del acceso y el uso de los productos de Adobe.
exl-id: bfee66b5-d7bb-4ecb-8d22-efb68611ecc8
source-git-commit: 6fcd91d09ffc23047b2fb332af256ab7706355cd
workflow-type: tm+mt
source-wordcount: '1689'
ht-degree: 100%

---

# Funciones de administrador

Con Adobe Admin Console, las organizaciones pueden definir una jerarquía administrativa flexible que permita una administración precisa del acceso y el uso de los productos de Adobe. Uno o más administradores del sistema, proporcionados durante el proceso de incorporación empresarial, ocupan la parte superior de la jerarquía. Estos administradores del sistema pueden delegar responsabilidades en otros administradores, manteniendo al mismo tiempo el control general.

Las funciones de administrador proporcionan a las empresas las siguientes ventajas clave:

* Descentralización controlada de las responsabilidades administrativas
* Vista rápida de las asignaciones de productos, por usuario y por producto
* Funcionalidad para asignar cuotas a los administradores de productos

## Jerarquía administrativa

Se aplica a: clientes empresariales de Adobe.

La jerarquía administrativa puede utilizarse para adaptarse a los requisitos únicos de su empresa. Por ejemplo, una empresa puede designar diferentes administradores para que gestionen las autorizaciones de las ofertas de Adobe Creative Cloud y Adobe Marketing Cloud. De manera alternativa, una empresa puede tener diferentes administradores para gestionar las autorizaciones de los usuarios que pertenecen a diferentes unidades de negocio.

>[!NOTE]
>
>La jerarquía administrativa no se aplica a los clientes de equipos. Los clientes de equipos tienen una sola función de **Administrador del sistema**. El propietario del contrato (_anteriormente denominado **Administrador principal**_) es el administrador del sistema con acceso a los detalles del contrato y al historial de facturación. Si es el propietario del contrato actual, puede designar un administrador del sistema existente (_ anteriormente denominado **administrador secundario**_) como propietario del contrato.

![imagen de administrador](assets/storage_admin.png)

_Jerarquía de funciones de administrador_

| Función | Descripción |
|--- |--- |
| **Administrador del sistema** | Superusuario de la organización; puede realizar todas las tareas administrativas en Admin Console.<br>Además, tiene permisos para delegar la siguiente funcionalidad administrativa en otros usuarios: administrador de productos, administrador de perfiles de producto, administrador de grupos de usuarios, administrador de implementación y administrador de asistencia. |
| **Administrador de productos** | Administra los productos asignados a ese administrador y todas las funciones administrativas asociadas, que incluyen:<ul><li>Crear perfiles de producto</li><li>Agregar usuarios y grupos de usuarios a la organización, pero no eliminarlos</li><li>Agregar o quitar usuarios y grupos de usuarios de perfiles de producto</li><li>Agregar o quitar administradores de perfiles de producto</li><li>Agregar o quitar otros administradores de productos</li><li>Agregar o quitar administradores de grupos</li></ul> |
| **Administrador del perfil de producto** | Administra las descripciones de perfil de producto asignadas a ese administrador y todas las funciones administrativas asociadas, que incluyen:<ul><li>Agregar usuarios y grupos de usuarios a la organización, pero no eliminarlos</li><li>Agregar o quitar usuarios y grupos de usuarios de perfiles de producto</li><li>Asignar o revocar permisos de producto para usuarios y grupos de usuarios desde perfiles de producto</li><li>Administrar funciones de producto de usuarios y grupos de usuarios para perfiles de producto |
| **Administrador del grupo de usuarios** | Administra las descripciones de grupo de usuarios asignadas a ese administrador y todas las funciones de administrador asociadas, que incluyen:<ul><li>Agregar o quitar usuarios de grupos</li><li>Agregar o quitar administradores de grupos de usuarios de grupos |
| **Administrador de implementación** | Crea, administra e implementa paquetes de software y actualizaciones para usuarios finales. |
| **Administrador de asistencia** | Función no administrativa que tiene acceso a información relacionada con la asistencia, como los informes de problemas notificados por el cliente. |
| **Administrador de almacenamiento** | Gestiona la administración del almacenamiento de la organización. El administrador puede ver el consumo de almacenamiento de los usuarios activos e inactivos y transferir el contenido a otros destinatarios. |

Para obtener una lista detallada de permisos y privilegios para cada función de administrador, consulte [Permisos](#enterprise-admins-permissions-matrix).

## Agregar una función de administrador de empresa {#add-enterprise-role}

Se aplica a: clientes empresariales de Adobe.

Como administrador, puede asignar una función de administrador a otros usuarios, otorgándoles los mismos privilegios que tiene, o privilegios para una función de su función de administrador en la jerarquía como se describe [arriba](#administrative-hierarchy). Por ejemplo, como administrador de producto, puede otorgar privilegios de administrador de producto o privilegios de administrador de perfil de producto a un usuario, pero no privilegios de administrador de implementación. Para obtener los permisos de Admin Console, consulte la [Guía de permisos](#enterprise-admins-permissions-matrix).

Para agregar o invitar a un administrador:

1. En [Admin Console](https://adminconsole.adobe.com/), elija **Usuarios** > **Administradores**.

   Como alternativa, vaya al producto, perfil de producto o grupo de usuarios correspondiente y a la pestaña **Administradores**.

1. Haga clic en **Agregar administrador**.
1. Introduzca un nombre o una dirección de correo electrónico. Puede buscar usuarios existentes o agregar un nuevo usuario especificando una dirección de correo electrónico válida y rellenando la información en la pantalla.
1. Haga clic en **Siguiente**. Aparece una lista de funciones de administrador.

>[!NOTE]
>
>* Las opciones de esta pantalla dependen de la cuenta y de la función de administrador. Puede otorgar los mismos privilegios que tiene, o privilegios para una función por debajo de la suya en la jerarquía.
>* Como administrador del sistema de un equipo, solo puede asignar una función de administrador: Administrador del sistema.

1. Seleccione una o varias funciones de administrador.
1. Para los tipos de administrador como Administrador de productos, Administrador de perfiles de producto y Administrador de grupos de usuarios, seleccione los productos, perfiles y grupos específicos, respectivamente.

>[!NOTE]
>
>Para un administrador de perfil de producto, puede incluir perfiles de más de un producto.

![agregar administrador](assets/add-admin.png)

1. Revise las funciones de administrador asignadas al usuario y haga clic en **Guardar**.

El usuario recibe una invitación por correo electrónico con respecto a los nuevos privilegios administrativos de `message@adobe.com`.

Los usuarios deben hacer clic en **Empezar** en el correo electrónico para unirse a la organización. Si los nuevos administradores no utilizan el enlace **Empezar** de la invitación por correo electrónico, no podrían iniciar sesión en Admin Console.

Como parte del proceso de inicio de sesión, es posible que se pida a los usuarios que configuren un perfil de Adobe si todavía no lo tienen. Si los usuarios tienen varios perfiles asociados a su dirección de correo electrónico, deben elegir &quot;Unirse al equipo&quot; (si se les solicita) y luego seleccionar el perfil asociado a la nueva organización.

![imagen de derechos de administrador](assets/admin-get-started-email.png)

## Agregar un administrador de equipos {#add-admin-teams}

Se aplica a: clientes de Adobe para equipos.

Como administrador, puede asignar la función de administrador del sistema a otros usuarios, otorgándoles los mismos privilegios que tiene.

Para agregar o invitar a un administrador del sistema:

1. En Admin Console, elija **Usuarios** > **Administradores**.

   Se muestra una lista de administradores existentes.

1. Haga clic en **Agregar administrador**.

   Se muestra la pantalla **Agregar un administrador**.

1. Introduzca un nombre o una dirección de correo electrónico. Puede buscar usuarios existentes o agregar un nuevo usuario especificando una dirección de correo electrónico válida y rellenando la información en la pantalla.

   De forma predeterminada, Administrador del sistema está seleccionado.

1. Haga clic en **Guardar**.

![imagen de administrador de equipos](assets/teams-admin.png)

Dado que todos los usuarios de una organización de equipos son usuarios de Business ID, reciben una invitación por correo electrónico con respecto a los nuevos privilegios administrativos de `message@adobe.com`.
Los usuarios deben hacer clic en Empezar en el correo electrónico para unirse a la organización.

Como parte del proceso de inicio de sesión, es posible que se pida a los usuarios que configuren un perfil de Adobe si todavía no lo tienen. Si los usuarios tienen varios perfiles asociados a su dirección de correo electrónico, deben elegir &quot;Unirse al equipo&quot; (si se les solicita) y luego seleccionar el perfil asociado a la nueva organización.

![imagen de derechos de administrador](assets/admin-get-started-email.png)

## Editar función de administrador empresarial

Se aplica a: clientes empresariales de Adobe.

Como administrador, puede editar la función de administrador a otros administradores que se encuentran debajo de usted en la jerarquía administrativa. Por ejemplo, puede eliminar los privilegios de administrador de otros administradores.

Para editar las funciones de administrador:

1. En Admin Console, elija **Usuarios** > **Administradores**. Se muestra la lista de administradores existentes.

   Como alternativa, vaya al producto, perfil de producto o grupo de usuarios correspondiente y a la pestaña **Administradores**.

1. Haga clic en el nombre del administrador que desea editar.
1. En **Detalles del usuario**, haga clic en el ![icono](assets/one-console-ellipses.png) para ver los **Derechos de administrador** y elija **Editar derechos de administrador**.

   ![editar derechos de administrador](assets/admin-rights-section.png)

1. Edite los derechos de administrador y guarde los cambios.

## Editar la función de administrador de equipos

Se aplica a: clientes de Adobe para equipos.

Como administrador del sistema de equipos, puede eliminar los privilegios de administrador del sistema de otros administradores.

Para revocar los privilegios de administrador del sistema:

1. En Admin Console, elija **Usuarios** > **Administradores**.

   Se muestra la lista de administradores existentes.

1. En Detalles del usuario, haga clic en el ![icono](assets/one-console-ellipses.png) a la derecha de **Derechos de administrador** y elija **Editar derechos de administrador**.

   ![editar derechos de administrador](assets/admin-rights-section.png)

1. Edite los derechos de administrador y guarde los cambios.

## Eliminar un administrador

Se aplica a: clientes empresariales de Adobe para equipos.

1. Para revocar permisos de administrador, seleccione un usuario y haga clic en **Eliminar administrador**.

![quitar imagen de administrador](assets/remove-admin.png)

>[!NOTE]
>
>Al eliminar un administrador, no se elimina el usuario de Admin Console, sino que solo se eliminan los privilegios asociados a la función de administrador.

## Guía de permisos de los administradores de empresa

Se aplica a: clientes empresariales de Adobe.

La siguiente tabla enumera todos los permisos para los distintos tipos de administradores, clasificados por las siguientes áreas de funcionalidad:

### Administración de identidades

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Añadir dominio (solicitar/reclamar un dominio) | ✔ | |
| Ver dominios y listado de dominios | ✔ | |
| Administrar claves de cifrado de dominio | ✔ | |
| Administrar la directiva de contraseñas de organización predeterminada | ✔ | |
| Ver directiva de contraseñas de organización predeterminada | ✔ | |

### Administración de usuarios

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Agregar usuario a organización | ✔ | |
| Eliminar usuario de organización | ✔ | |
| Ver detalles de usuario y listado | ✔ | |
| Editar perfil de usuario | ✔ | |
| Agregar perfil de producto al usuario o grupo | ✔ | |
| Eliminar perfil de producto del usuario o grupo | ✔ | |
| Agregar perfil de producto a varios usuarios | ✔ | |
| Ver perfiles de producto para un usuario | ✔ | |
| Ver lista de usuarios del producto | ✔ | |
| Agregar grupo de usuarios a la organización | ✔ | |

### Gestión de administradores

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Otorgar la función de administrador de organización a un usuario | ✔ | |
| Revocar el administrador de organización de un usuario | ✔ | |
| Otorgar la función de administrador de licencias de producto a un usuario | ✔ | |
| Revocar el administrador de licencias de producto de un usuario | ✔ | |
| Otorgar la función de administrador de implementación a un usuario | ✔ | |
| Revocar el administrador de implementación de un usuario | ✔ | |
| Otorgar la función de administrador de grupos de usuarios a un usuario | ✔ | |
| Revocar la función de administrador de grupos de usuarios de un usuario | ✔ | |
| Otorgar la función de administrador de propietario de producto a un usuario | ✔ | |
| Revocar el administrador del propietario del producto de un usuario | ✔ | |

### Administración de la configuración de la licencia del producto

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Otorgar derechos de producto a organización | | |
| Eliminar la asignación de productos de la organización | | |
| Ver el número total de licencias propiedad de la organización | ✔ | |
| Ver productos disponibles y familias de productos | ✔ | |
| Editar descripciones/datos de licencias de productos | ✔ | |
| Proporcionar licencia de producto a un usuario | ✔ | |
| Cancelar la licencia de producto de un usuario | ✔ | |
| Añadir nueva configuración de licencia de producto | ✔ | |
| Editar la configuración del servicio de licencias de producto | ✔ | |
| Eliminar la configuración del servicio de licencias de producto | ✔ | |
| Eliminar el acceso al producto de un usuario (eliminación de todas las configuraciones) | ✔ | |

### Administración del almacenamiento

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Ver carpetas de usuario activas e inactivas | ✔ | |
| Eliminar carpetas de usuario inactivas y transferir contenido | ✔ | |

### Implementación

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Pestaña Ver/usar paquetes | ✔ | |

### Asistencia técnica

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Ver pestaña de asistencia técnica | ✔ | |
| Administrar casos de asistencia técnica | ✔ | ✔ |

### Administración de grupos de usuarios

| Permiso | Administrador del sistema | Administrador de asistencia |
|--- |--- |--- |
| Crear grupo de usuarios | ✔ | |
| Eliminar grupo de usuarios | ✔ | |
| Agregar usuario al grupo de usuarios | ✔ | |
| Eliminar usuario del grupo de usuarios | ✔ | |
| Asignar grupo de usuarios a una licencia de producto | ✔ | |
| Eliminar grupo de usuarios de la licencia del producto | ✔ | |
| Ver miembro del grupo de usuarios | ✔ | ✔ |
| Ver lista de grupos de usuarios | ✔ | ✔ |
