---
description: P4 Warehouse - Agregar Zonas y Espacios (Bins)
---

# Agregar Zonas y Espacios

### Agregar Zona

En la pantalla de edición del almacén, haz clic en el botón :new: en la sección de Zonas de la pantalla.

{% hint style="info" %}
Para información más detallada sobre [Zonas](../../setup/warehouse/zones.md).
{% endhint %}

Después de hacer clic en Nuevo, aparecerá la pantalla de configuración. Completa el código de zona, la máscara, la descripción y el Tipo de Manejo de Producto, luego haz clic en Guardar.

{% hint style="info" %}
Los tipos de manejo de producto son: Por Producto o Por LPN (Placa de Identificación de Unidad Logística). Si no utilizas LPN, no selecciones LPN como tipo de manejo.
{% endhint %}

### Pantalla de Nueva Zona

Ahora verás tu nueva zona en la lista de zonas debajo de la pantalla de configuración del almacén.

Abre tu nueva zona haciendo clic en el enlace de la columna Código. Aquí configurarás los detalles de la zona.

En la pantalla de configuración de zona, encontrarás varias configuraciones detalladas para el comportamiento de la zona.

{% hint style="info" %}
Configurar una zona como cuarentena impedirá que puedas asignar el inventario de esa zona a pedidos.
{% endhint %}

La **Máscara de Zona** es una función especialmente importante, mejor administrada por el equipo de implementación. En resumen, la máscara de zona te ayuda a crear cientos o miles de ubicaciones de espacios automáticamente.

Estructura de la Máscara: los segmentos de la máscara van dentro de { }, cada segmento está numerado. A continuación algunos ejemplos con sus resultados:

* 01-A-{0:00}-{1:0} = 01-A-12-A
  * Este formato es: pasillo, zona, espacio, nivel
* A-{0:00}-{1:0} = A-03-A
  * Este formato es: zona, espacio, nivel

El enmascaramiento de zonas depende del diseño físico de tu almacén. Usa esta función con cuidado, ya que podrías crear accidentalmente cientos de miles de ubicaciones.

> No es obligatorio incluir la Zona en el formato de la etiqueta; la zona puede incluirse como un campo separado en la etiqueta del espacio.

Configurar la zona con espacios dedicados por producto es para casos de uso excepcionales y no se recomienda para la mayoría de los almacenes o centros de distribución.

{% hint style="success" %}
Es importante configurar la impresora de tickets de recolección en cada zona. Esto es fundamental si planeas usar la recolección por zona.

Las dimensiones de Zonas/Espacios son **vitales** para varios propósitos del sistema.
{% endhint %}

Al diseñar tus zonas, ten en cuenta: Zonas de Clasificación (Staging), Zonas de Tránsito Directo (Cross Dock), Zonas de Recepción, Zonas Refrigeradas, Zonas Congeladas, Zonas de Materiales Peligrosos, etc.
