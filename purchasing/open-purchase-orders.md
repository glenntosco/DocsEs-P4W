---
description: P4 Warehouse - Órdenes de Compra Abiertas
---

# Órdenes de Compra Abiertas

La página de OC Pendientes (Órdenes de Compra) muestra un listado de todas las órdenes de compra pendientes en el sistema WMS. Incluye columnas para: Casilla de Selección, Estado, Número de OC, Proveedor, Cliente, Almacén, Designación, Muelle, Número de Cita, Fecha de Cita y Fecha de Creación. También hay cuatro botones en la parte superior derecha:

- **Ingreso de Datos** — con dos opciones: Nuevo (crear una nueva OC) y A Borrador (asignar una OC seleccionada a estado borrador).
- **Recepción** — con tres opciones: Liberar al Piso (sacar una OC del estado borrador y convertirla en una tarea activa), Asignar Operario (asignar una OC a un operario específico) y Asignar Puerta de Muelle (asignar una OC a una puerta de muelle específica).
- **Otros** — con dos opciones: Correo Electrónico (para enviar notificación por email a un tercero) y Eliminar (eliminar una OC seleccionada).
- **Actualizar** — para refrescar la lista después de cualquier cambio.

Para crear una nueva orden de compra, selecciona el botón **Ingreso de Datos** y elige la opción Nuevo. Aparecerá una ventana emergente con opciones para Proveedor, Almacén y Número de OC. Selecciona el Proveedor y el Almacén de los menús desplegables. Ingresa un número de OC manualmente o deja el campo vacío (el sistema generará uno automáticamente). Selecciona el botón **Guardar** y P4 Warehouse abrirá la página de la Orden de Compra.

Para editar una orden de compra existente, selecciona el número de OC en la lista. El sistema abrirá la página de perfil de esa OC. En la parte superior derecha, la opción **Auditoría...** proporciona un registro cronológico completo de todos los eventos relacionados con esta OC. La sección de Encabezado permite editar Proveedor, Almacén, Referencia y Comentarios. A la derecha está la sección de Cita, donde se puede asignar un Transportista, número de transportista, fecha programada, puerta de muelle y el operario responsable.

Cerca de la parte inferior de la página está la sección de **Líneas**, que detalla todos los artículos de la orden de compra. Incluye columnas para: imagen miniatura, Producto, Descripción, Tamaño de Empaque (Packsize), Paquetes, Cantidad y Acción. Los tres botones en la esquina superior derecha de la OC son:

- **Actualizar** — guarda los cambios realizados en el perfil.
- **Liberar al Piso** — pone la OC en estado activo (normalmente "No Recibido"). Todas las OC están en estado Borrador hasta que se selecciona este botón.
- **A Borrador** — revierte la OC de vuelta a estado Borrador (disponible una vez liberada).
