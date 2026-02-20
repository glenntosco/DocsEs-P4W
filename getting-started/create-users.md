---
description: P4 Warehouse - Creación de Usuarios
---

# Crear Usuarios

Para crear un [nuevo usuario](../permissions/add-users.md), navega a Configuración > Sistema > Usuarios.

El menú de Usuarios lista las distintas cuentas de usuario creadas. Las cuentas de usuario pueden ser de tipo Administrador o tipo Usuario. Se pueden crear nuevos usuarios seleccionando el botón "Nuevo" en la parte superior derecha, o eliminar usuarios existentes seleccionando la "X" negra a la derecha de cada usuario listado (se pueden eliminar cuentas de Administrador adicionales, pero no la cuenta de Administrador inicial). Para examinar o editar un usuario existente, simplemente selecciona el nombre de usuario de la lista.

Desde la lista de usuarios de P4 Warehouse puedes realizar varias tareas:

* Agregar nuevo usuario
* Activar un usuario desactivado
* Desactivar un usuario
* Eliminar un usuario

También puedes suplantar (hacer clic en el ícono de enlace) a un usuario para verificar permisos y ayudar con la configuración de pantallas.

En la pantalla de Lista de Usuarios, puedes abrir y editar un usuario existente haciendo clic en el enlace de la columna de usuario, o puedes hacer clic en el botón :new: para agregar un nuevo usuario.

En la Pantalla de Configuración de Usuario hay varias secciones importantes que deben configurarse:

**Credenciales de inicio de sesión** — En esta sección configuras los ajustes básicos del usuario: nombre de usuario, contraseña, idioma, almacén predeterminado y permisos principales.

**Zonas Asignadas** — En esta área establece las zonas en las que el usuario está autorizado a trabajar. Esto evita que los usuarios trabajen fuera del almacén o zona asignada.

**Información personal** — Nombre, apellido, zona horaria y foto del usuario.

**Dispositivo portátil (Handheld)** — Esta configuración solo debe usarse para vehículos de la empresa que realizan entregas propias.

**Módulos** — Aquí se configuran los permisos según el rol del usuario en el almacén.

**Clientes** — Esta configuración es para un usuario que trabaja para un cliente 3PL específico. Limitará al usuario a ver solo los clientes, proveedores, órdenes de venta y órdenes de compra de ese cliente 3PL.

**Impresoras** — En esta sección elige la(s) impresora(s) que el usuario puede utilizar. Después de seleccionar las impresoras correspondientes, marca una como predeterminada. En la esquina inferior derecha hay un botón Avanzado para asignar diferentes impresoras a diferentes etiquetas.

**Menú predeterminado** — Determina la pantalla que se muestra al iniciar sesión. Por ejemplo: /demolatam/main/pickTicketList/true abrirá la pantalla de pedidos pendientes para el Tenant Demolatam.

{% hint style="danger" %}
**¡Usa esto con precaución! Ingresar datos inválidos aquí puede bloquear al usuario y dejarlo sin acceso al sistema.**
{% endhint %}
