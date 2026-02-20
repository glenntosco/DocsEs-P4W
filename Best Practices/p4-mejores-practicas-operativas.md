# P4 Warehouse — Guía de Mejores Prácticas Operativas

## Para quién es esta guía

Esta guía es para todos los que trabajan en un almacén — desde el gerente de bodega que planifica el día, hasta el receptor en el muelle, el recolector que camina entre los pasillos, y el supervisor que verifica los envíos.

No necesitas ser experto en tecnología para usar P4 Warehouse correctamente. Solo necesitas entender *por qué* se hacen las cosas de cierta manera, y *cómo* hacerlas en el sistema. Eso es exactamente lo que cubre esta guía.

> 💡 **Cómo usar esta guía:** Busca tu rol o tu tarea. Lee primero la sección "Por qué importa" — entender el motivo hace que sea más fácil recordar los pasos. Luego sigue las instrucciones paso a paso para P4 Warehouse.

---

## Tabla de Contenidos

1. [Recepción de Mercancía](#recepción-de-mercancía)
2. [Almacenamiento (Putaway)](#almacenamiento-putaway)
3. [Recolección de Pedidos (Picking)](#recolección-de-pedidos-picking)
4. [Empaque y Envío](#empaque-y-envío)
5. [Conteo Cíclico](#conteo-cíclico)
6. [Devoluciones (RMA)](#devoluciones-rma)
7. [Gestión de Inventario](#gestión-de-inventario)
8. [Logística para Terceros (3PL)](#logística-para-terceros-3pl)
9. [Métricas de Desempeño](#métricas-de-desempeño)
10. [Capacitación y Mejora Continua](#capacitación-y-mejora-continua)

---

## Recepción de Mercancía

### ¿Qué es la recepción?

La recepción es el primer paso en tu almacén. Cuando llega un camión con productos, tu trabajo es contar lo que llegó, revisar su condición, ingresarlo a P4 Warehouse y moverlo a una ubicación de almacenamiento. Si cometes un error aquí, ese error te seguirá en cada paso posterior.

**Por qué importa la exactitud en la recepción:** Si recibes 100 cajas pero solo escaneas 90 en el sistema, tu inventario ya está incorrecto. Cuando un cliente pida esas 10 cajas faltantes, el sistema dirá que las tienes — pero no las tendrás. Eso significa un envío tardío y un cliente insatisfecho.

---

### Antes de que llegue el camión

**¿Por qué planificar con anticipación?** Programar las llegadas al muelle evita que los camiones se acumulen al mismo tiempo, dejando a los conductores esperando y a tu equipo sobrepasado.

**En P4 Warehouse:**
Ve a **Compras → Calendario de Recepción** para ver qué se espera hoy. Usa la vista de citas para distribuir las llegadas a lo largo de tu turno.

✅ **Haz esto:**
- Saber qué viene antes de que llegue (revisa el calendario cada mañana)
- Asignar una puerta de muelle específica a cada entrega esperada
- Tener pallets vacíos, etiquetas y un escáner funcionando listos en el muelle
- Asegurarte de tener una copia impresa de la Orden de Compra (OC) como respaldo

❌ **No hagas esto:**
- Aceptar una entrega sin una OC en el sistema
- Dejar que dos entregas grandes lleguen al mismo tiempo sin personal adicional

---

### Paso a paso: recibir un envío en P4

**En la web (para supervisores/oficina):**
1. Ve a **Recepción → Órdenes de Compra**
2. Encuentra la OC para este envío y ábrela
3. Haz clic en **Recibir** para iniciar el proceso
4. Asigna un receptor y una puerta de muelle

**📱 En el dispositivo portátil (para trabajadores del muelle):**
1. Abre la aplicación móvil de P4
2. Ve a **Recepción → Recepción de OC**
3. Escanea el código de barras de la OC o ingresa el número de OC
4. Escanea el código de barras de cada producto e ingresa la cantidad recibida
5. El sistema te dirá dónde guardarlo (ubicación de almacenamiento)
6. Cuando termines, confirma y cierra la OC

> ⚠️ **Cuidado:** Nunca cierres una OC hasta que todos los productos estén físicamente en una ubicación. Si la cierras antes, el sistema cree que está terminada — pero el producto todavía está en el muelle.

---

### Situaciones especiales en la recepción

#### Productos con fechas de vencimiento (como alimentos, medicamentos o químicos)

**Por qué importa:** Vender un producto vencido a un cliente es un problema serio — legal y para su seguridad. Capturamos las fechas de vencimiento en la recepción para que el sistema automáticamente venda primero el producto que vence más pronto (esto se llama FEFO — *First Expired, First Out*, o sea, el primero en vencer es el primero en salir).

**📱 En el dispositivo portátil:**
Al recibir un producto con fecha de vencimiento, la aplicación te pedirá el número de lote y la fecha de vencimiento. Siempre ingresa la fecha exacta que aparece en la etiqueta del producto.

✅ **Haz esto:**
- Revisar la fecha de vencimiento en cada caja/unidad antes de escanear
- Si un producto ya está vencido o vence muy pronto, apártalo e informa a tu supervisor de inmediato
- Poner el stock más nuevo detrás del más viejo en el estante (para que el producto más antiguo se recolecte primero)

❌ **No hagas esto:**
- Saltar el campo de fecha de vencimiento — el sistema lo requiere por una razón
- Mezclar diferentes números de lote en el mismo espacio (bin)

---

#### Productos vendidos por peso (como químicos a granel, tela o cable)

**Por qué importa:** Si el sistema dice que recibiste 100 kg pero solo recibiste 95 kg, tu inventario está mal desde el primer día. Los productos a base de peso deben pesarse con exactitud en la recepción.

✅ **Haz esto:**
- Usar una báscula calibrada (verifica que haya sido calibrada recientemente)
- Poner a cero la báscula con el contenedor vacío antes de pesar (esto se llama "tarar")
- Ingresar el peso con dos decimales
- Una pequeña diferencia (hasta el 2%) es normal — documenta cualquier diferencia mayor

---

### Errores comunes en la recepción

| Error | Qué sale mal | Cómo evitarlo |
|-------|-------------|---------------|
| No escanear todos los productos | El inventario empieza incorrecto | Escanea cada artículo, sin excepciones |
| Recibir en la OC equivocada | Genera confusión en el inventario | Siempre confirma el número de OC antes de escanear |
| Saltarse las fotos de daños | No se puede reclamar al transportista después | Fotografía cualquier daño antes de firmar la entrega |
| Cerrar la OC antes de guardar | El sistema cree que el producto está disponible antes de que esté ubicado | Espera hasta que se confirme el almacenamiento |
| Ignorar las fechas de vencimiento | Producto vencido entra al stock | Siempre revisa e ingresa las fechas |

---

## Almacenamiento (Putaway)

### ¿Qué es el almacenamiento?

El almacenamiento es mover el producto recibido desde el muelle hasta su ubicación de almacenaje. El lugar donde pones algo importa — mucho. Poner productos de alta rotación en lugares de difícil acceso ralentiza a tus recolectores todos los días.

---

### ¿Dónde deben ir los productos?

**La regla de la zona dorada:** La zona más fácil para recolectar está entre tu cintura y tus hombros. Pon tus productos más populares ahí. Los menos populares van más arriba, más abajo o más lejos.

**Cómo saber qué es popular:** Pide a tu supervisor un reporte de frecuencia de recolección (**Analítica → Reportes**). Los productos más recolectados deben estar en las mejores ubicaciones.

**Pautas generales:**

| Tipo de producto | Dónde ponerlo |
|-----------------|---------------|
| Recolectado todos los días | Zona dorada, más cerca del área de empaque |
| Recolectado algunas veces a la semana | Estante estándar, distancia media |
| Recolectado raramente | Estante superior, parte trasera del almacén, almacenaje a granel |
| Productos pesados | Siempre a nivel del piso o estante bajo |
| Productos frágiles | Zona separada, claramente marcada |
| Productos de alto valor | Área segura con acceso limitado |

---

### Cómo P4 guía el almacenamiento

P4 Warehouse puede sugerir o indicar dónde poner los productos basándose en reglas que tu administrador configura.

**📱 En el dispositivo portátil:**
Después de recibir, la aplicación hará una de estas cosas:
- **Te dirá exactamente a dónde ir** (almacenamiento dirigido) — solo sigue las instrucciones
- **Sugerirá una ubicación** — puedes aceptarla o elegir una diferente
- **Te dejará elegir** — escanea la ubicación que quieras y confirma

> 💡 **Consejo:** Siempre escanea el código de barras del espacio al guardar el producto — no solo escribas la ubicación. Escanear confirma que estás en el lugar correcto.

---

### Mejores prácticas de almacenamiento

✅ **Haz esto:**
- Siempre escanear el código de barras del espacio para confirmar la ubicación
- Poner productos similares juntos (productos que se piden frecuentemente juntos deben estar cerca)
- Si una ubicación está llena, informa a tu supervisor — no comprimas producto en un espacio desbordado
- Para productos con fecha de vencimiento, coloca el stock más nuevo *detrás* del más viejo

❌ **No hagas esto:**
- Poner un producto donde sea conveniente sin actualizar el sistema
- Mezclar diferentes productos en un espacio marcado para un solo SKU (SKU = código de producto)
- Dejar producto en el muelle "por un momento" — se vuelve invisible para los recolectores

---

## Recolección de Pedidos (Picking)

### ¿Qué es la recolección?

La recolección es ir a la ubicación de un producto y tomarlo para empacarlo para un pedido de cliente. La velocidad y la exactitud importan. Un artículo mal recolectado llega al cliente como un envío incorrecto — costoso y frustrante para todos.

---

### Métodos de recolección en P4

P4 Warehouse soporta varios métodos de recolección. Tu supervisor configurará cuál usa tu almacén.

| Método | Cómo funciona | Mejor para |
|--------|--------------|-----------|
| **Recolección por pedido individual** | Recolectar un pedido a la vez | Operaciones pequeñas, pedidos grandes y complejos |
| **Recolección por ola (Wave)** | Un grupo de pedidos se libera a la vez; los recolectores trabajan toda la ola | Operaciones de alto volumen |
| **Recolección en lote (Batch)** | Un recolector recoge artículos para múltiples pedidos en un solo recorrido | Muchos pedidos pequeños con productos similares |
| **Recolección de cartones** | Recolectar cajas completas — sin necesidad de desglosarlas | Pedidos B2B, envíos de cajas completas |

---

### Recolección por ola — cómo funciona

Una "ola" es un grupo de pedidos liberados para recolección al mismo tiempo. Tu supervisor crea la ola en P4 y la asigna a los recolectores.

**En P4 (supervisor — web):**
1. Ve a **Despacho → Lista de Recolección**
2. Selecciona los pedidos a incluir en la ola
3. Haz clic en **Ola** y configura los ajustes
4. Libera la ola — los recolectores la verán en sus dispositivos portátiles

**📱 En el dispositivo portátil (recolector):**
1. Abre la aplicación móvil de P4
2. Ve a **Recolección → Recolección por Ola**
3. Selecciona tu ola asignada
4. Sigue el sistema — te guiará a cada ubicación en el orden más eficiente
5. Escanea el código de barras del producto para confirmar cada recolección
6. Coloca en el contenedor correcto (la aplicación te dice cuál)

> 💡 **Consejo:** Siempre sigue el orden que te da el sistema. Está diseñado para minimizar el caminar. Si saltas de un lugar a otro, caminarás más y recolectarás menos.

---

### Recolección paso a paso (pedido individual)

**📱 En el dispositivo portátil:**
1. Ve a **Recolección → Recolección por Ticket**
2. Escanea o selecciona tu ticket de recolección
3. Ve a la primera ubicación que muestra la aplicación
4. Escanea el código de barras del espacio para confirmar que estás en el lugar correcto
5. Escanea el código de barras del producto
6. Ingresa la cantidad (o confirma si ya está precargada)
7. Coloca el producto en tu contenedor (tote)
8. Repite hasta completar el ticket de recolección
9. Lleva el contenedor al área de clasificación (staging)

---

### Recolección de productos especiales

#### Productos con fecha de vencimiento (FEFO)

FEFO significa **Primero en Vencer, Primero en Salir** — siempre recolecta primero el producto que vence *más pronto*.

**P4 lo aplica automáticamente:** El sistema te dirá qué lote recolectar. Debes escanear la etiqueta del lote correcto para confirmar.

> ⚠️ **Cuidado:** Si el sistema te pide recolectar el Lote A pero tú recolectas el Lote B porque es más conveniente, estás violando el FEFO. Esto puede llevar a que producto vencido llegue a los clientes. El sistema lo detectará — no intentes saltarte este paso.

#### Productos por peso

**📱 En el dispositivo portátil:**
1. Ve a la ubicación
2. Pesa la cantidad requerida en la báscula
3. Ingresa el peso real que recolectaste
4. Imprime una etiqueta de peso y pégala al contenedor
5. El sistema acepta una pequeña variación (generalmente ±2%)

---

### Consejos para exactitud en la recolección

✅ **Haz esto:**
- Escanear cada código de barras — no supongas
- Si una ubicación está vacía o el producto no coincide, detente y llama a tu supervisor
- Contar la cantidad antes de confirmar
- Mantener tus contenedores organizados — un contenedor por pedido a menos que el sistema indique lo contrario

❌ **No hagas esto:**
- Recolectar un producto "parecido" y asumir que está bien
- Saltarte el escaneo e ingresar cantidades manualmente
- Dejar un ticket de recolección a medias sin reportarlo

---

## Empaque y Envío

### Empaque

El empaque es preparar el pedido para salir del almacén. Un pedido bien empacado llega intacto y a tiempo. Un pedido mal empacado puede dañarse en tránsito — y eso es un problema que tu almacén tiene que resolver.

**Reglas básicas de empaque:**
- Usa el tamaño de caja correcto — una caja demasiado grande desperdicia espacio y permite que el producto se mueva y se dañe
- Rellena el espacio vacío (con plástico burbuja, papel o relleno de espuma)
- Los artículos frágiles necesitan relleno adicional y a veces una etiqueta de "Frágil"
- Sella la caja completamente — las solapas sueltas se abren en tránsito

**En P4:** El sistema puede sugerir un tamaño de caja basado en las dimensiones del pedido (esto se llama cartonización). Usa el tamaño sugerido a menos que tengas una razón clara para no hacerlo.

---

### Métodos de envío

P4 Warehouse soporta diferentes formas de enviar. Tu administrador configura qué transportistas y métodos están disponibles.

| Tipo de envío | Cuándo usarlo | Ejemplo |
|--------------|--------------|---------|
| **Paquetería (Small Parcel)** | Cajas individuales, peso ligero | UPS, FedEx, DHL |
| **Carga consolidada (LTL)** | Envíos de tamaño de pallet, camión compartido | Transportistas de carga regional |
| **Camión completo (FTL)** | Llenarás todo el camión | Pedidos grandes, envíos a granel |
| **Flota privada** | Los camiones de tu propia empresa | Entregas locales o regionales |

> 💡 **¿Qué es LTL (Carga Consolidada)?** Significa que tu envío comparte un camión con la mercancía de otras empresas. Es más económico que rentar un camión completo, pero tarda más.

---

### Enviar un ticket de recolección en P4

**📱 En el dispositivo portátil:**
1. Ve a **Despacho → Envío**
2. Escanea el ticket de recolección o el contenedor
3. Confirma el transportista y el nivel de servicio
4. Escanea el contenedor a la puerta de muelle
5. Genera la etiqueta del transportista (si es paquetería)
6. Envía y cierra

**En la web (supervisor):**
1. Ve a **Despacho → Envío de Tickets de Recolección**
2. Selecciona el ticket de recolección
3. Confirma los detalles del envío
4. Haz clic en **Enviar**

---

### Cargas de camión (Truck Loads)

Cuando múltiples pedidos salen en el mismo camión, P4 los agrupa en una **Carga de Camión**. La carga de camión tiene un **Conocimiento de Embarque (BOL)** — el documento que viaja con el envío.

**📱 Para enviar una carga de camión:**
1. Ve a **Despacho → Envío de Cargas de Camión**
2. Selecciona la carga de camión
3. Confirma que todos los contenedores/pallets están cargados
4. Ingresa el nombre del conductor y el número de seguimiento (PRO) si es requerido
5. Genera e imprime el Conocimiento de Embarque
6. Envía

---

## Conteo Cíclico

### ¿Qué es un conteo cíclico?

Un conteo cíclico es una verificación regular del inventario — en lugar de contar todo a la vez (lo que toma días), cuentas pequeñas secciones del almacén regularmente. Esto mantiene tu inventario exacto sin detener las operaciones.

**Por qué importa:** Un inventario inexacto causa faltantes (crees que tienes algo pero no lo tienes), exceso de stock (sigues comprando algo de lo que ya tienes demasiado), y pedidos incorrectos enviados a clientes.

---

### Con qué frecuencia contar

No todos los productos necesitan contarse con igual frecuencia. Cuenta tus productos más importantes y más activos con mayor regularidad.

| Categoría de producto | Con qué frecuencia contar |
|----------------------|--------------------------|
| Artículos de alto valor o alta rotación | Mensualmente |
| Artículos de rotación media | Cada 3 meses |
| Artículos de baja rotación | Una vez al año |

> 💡 **Regla simple:** Si un producto se mueve mucho, cuéntalo seguido. Si apenas se mueve, cuéntalo ocasionalmente.

---

### Cómo hacer un conteo cíclico en P4

**En P4 Warehouse, hay tres formas de contar:**

1. **Por espacio (bin)** — Cuenta todo lo que hay en un espacio o área específica
2. **Por producto** — Cuenta todas las ubicaciones que tienen un producto específico
3. **Por asignación** — Cuenta una lista de artículos que te asignó un supervisor

**📱 En el dispositivo portátil:**
1. Ve a **Varios → Conteo Cíclico**
2. Elige tu tipo de conteo (por espacio, por producto o por asignación)
3. Escanea el código de barras del espacio o ingresa el producto
4. Cuenta todo lo que veas en esa ubicación
5. Ingresa la cantidad
6. Envía — el sistema marcará cualquier diferencia

**Importante:** El sistema NO te mostrará qué cantidad espera. Esto se llama **conteo a ciegas** — se hace así a propósito para que no solo confirmes el número que muestra el sistema. Cuenta lo que realmente hay.

---

### Cuando hay una diferencia

Si tu conteo no coincide con lo que tiene el sistema, este lo marcará como una variación. Una pequeña diferencia (1-2 artículos) puede ser un error normal. Una diferencia grande necesita investigación.

**Pasos cuando encuentras una diferencia:**
1. Vuelve a contar el espacio (puede que hayas contado mal)
2. Verifica si hay producto en otro espacio cercano
3. Revisa los artículos recibidos recientemente (puede que algo no se escaneó correctamente)
4. Reporta a tu supervisor — él revisará y aprobará el ajuste

> ⚠️ **Cuidado:** Nunca ajustes el inventario sin aprobación del supervisor. Los ajustes de inventario se registran, y los cambios no autorizados son una señal de alerta.

---

## Devoluciones (RMA)

### ¿Qué es una devolución (RMA)?

RMA significa **Autorización de Devolución de Mercancía** — es el sistema para manejar productos que regresan de los clientes. Manejar las devoluciones rápida y exactamente mantiene a los clientes satisfechos y devuelve el producto utilizable al stock.

---

### El proceso de devoluciones en P4

**Crear una devolución (web — servicio al cliente):**
1. Ve a **Devoluciones → Devoluciones Abiertas → Nueva Devolución**
2. Ingresa el cliente y los productos que se devuelven
3. Selecciona el motivo de la devolución
4. Guarda — se genera un número de devolución
5. El almacén recibe notificación para esperar la devolución

**Recibir una devolución (dispositivo portátil — trabajador del muelle):**
1. Ve a **Devoluciones → Recepción de RMA** en el dispositivo portátil
2. Escanea el código de barras del RMA
3. Inspecciona la condición del producto
4. Toma una foto si hay algún daño
5. Ingresa las cantidades recibidas
6. Confirma — el sistema te dirá dónde guardarlo según su condición

---

### Qué hacer con los productos devueltos

No todas las devoluciones regresan al stock. Inspecciona cada una y elige la acción correcta:

| Condición | Acción |
|-----------|--------|
| Sin abrir, en perfectas condiciones | Regresar al stock — mismo espacio que el producto nuevo |
| Abierto pero completo y limpio | Inspeccionar, probar si es posible, luego regresar al stock secundario |
| Dañado | Documentar con fotos, apartar para reclamación al proveedor |
| Producto incorrecto recibido (error nuestro) | Regresar al stock, investigar el error de recolección |
| Defectuoso | Apartar para devolución al proveedor o eliminación |

---

### Tomar fotos de las devoluciones

P4 Warehouse te permite adjuntar fotos a un registro de devolución. Siempre toma una foto cuando:
- El producto está dañado
- El empaque está faltante o destruido
- El cliente afirma que había algo mal con el producto

Esta foto se convierte en tu evidencia si hay una disputa con el cliente o el transportista.

**📱 En el dispositivo portátil:** La pantalla de Recepción de RMA tiene una opción de **Foto** — úsala.

---

## Gestión de Inventario

### Mantener el inventario exacto

El número de inventario en P4 debe coincidir siempre con lo que hay físicamente en el estante. Cuando no coinciden, los pedidos salen mal.

**Las tres principales causas de errores de inventario:**
1. Productos recibidos pero no escaneados en el sistema
2. Productos recolectados incorrectamente (producto o cantidad equivocada)
3. Productos dañados, vencidos o perdidos sin registrar

**Prevenir es mejor que corregir.** La mejor manera de mantener el inventario exacto es escanear correctamente cada vez — al recibir, al recolectar y al enviar.

---

### Niveles mínimo y máximo — tener la cantidad correcta en stock

Los niveles mínimo y máximo le dicen a P4 cuándo alertarte para reordenar.

- **Mínimo:** La cantidad más baja que debes tener. Cuando el stock baja a este nivel, es hora de reordenar.
- **Máximo:** La cantidad máxima que debes almacenar. Cuando recibes un envío, generalmente repones hasta este nivel.

**Regla simple para fijar el mínimo:** Piensa en cuánto tarda tu proveedor en entregar. Si tarda 5 días y usas 10 unidades por día, necesitas al menos 50 unidades como mínimo. Agrega algunos días extra como margen para retrasos.

**En P4 (administrador):** Ve a **Configuración → Almacén → Espacios** para fijar los niveles mínimo y máximo por espacio.

---

### Gestión de fechas de vencimiento

**La regla es simple: el producto más viejo sale primero (FEFO).**

P4 aplica el FEFO automáticamente durante la recolección — los recolectores son dirigidos al lote que vence más pronto. Tu trabajo es asegurarte de:

1. Siempre ingresar las fechas de vencimiento correctamente al recibir
2. Almacenar el stock más nuevo detrás del más viejo
3. Revisar regularmente los productos próximos a vencer

**Alertas de próximo vencimiento:** P4 puede marcar productos que se acercan a su vencimiento. Tu administrador las configura en **Configuración → Productos** para cada tipo de producto.

**Si encuentras producto vencido:**
- Retíralo del espacio inmediatamente
- Márcalo en el sistema con un ajuste (negativo) y motivo "Vencido"
- Obtén la aprobación del supervisor para el ajuste
- Elimina de manera apropiada

---

### Inventario de baja rotación

Los productos que no se han movido en 3-6 meses son un problema. Ocupan espacio y, si tienen fechas de vencimiento, pueden vencer antes de que alguien los compre.

**📊 Cómo encontrar productos de baja rotación:** Pide a tu supervisor un reporte de movimiento en **Analítica → Reportes**. Filtra por productos sin recolecciones en los últimos 90 días.

**Qué hacer con los artículos de baja rotación:**
1. Habla con el equipo de ventas — ¿pueden promoverlos o hacer un descuento?
2. Verifica si están próximos a vencer
3. Considera devolverlos al proveedor
4. Si no pueden venderse ni devolverse, elimínalos apropiadamente y registra el ajuste

---

## Logística para Terceros (3PL)

### ¿Qué es 3PL?

3PL significa **Logística de Terceros** — significa que tu almacén almacena y envía productos para otras empresas (tus clientes). El inventario de cada cliente está separado, y les cobras por los servicios que les brindas.

---

### Incorporar un nuevo cliente

Cuando tomas un nuevo cliente 3PL, hay pasos para configurarlo en P4 antes de que llegue su inventario:

**Semana 1 — Configuración:**
1. Crear el perfil del cliente: **Configuración → 3PL → Clientes → Nuevo Cliente**
2. Configurar tarifas y perfiles de facturación
3. Asignar zonas/espacios del almacén para su inventario
4. Crear cuentas de usuario para su equipo
5. Importar su catálogo de productos

**Semana 2 — Pruebas:**
1. Hacer una recepción de prueba con producto de muestra
2. Procesar algunos pedidos de muestra de principio a fin
3. Ejecutar un cálculo de facturación y verificar que sea correcto
4. Guiar al cliente a través de cómo usar su portal

**Semana 3 — Inicio de operaciones:**
1. Transferir su inventario real
2. Habilitar cualquier integración (flujos de pedidos, etc.)
3. Monitorear la primera semana de cerca — verificar diariamente

---

### Mantener el inventario de los clientes separado

El producto de cada cliente debe permanecer física y sistemáticamente separado.

**Separación física:** Asigna zonas o pasillos dedicados a cada cliente. Usa señalización clara.

**Separación en el sistema:** P4 rastrea automáticamente el inventario por cliente — siempre verás a qué cliente pertenece cada producto al recibir, recolectar y enviar.

> ⚠️ **Cuidado:** Nunca pongas el producto del Cliente A en la ubicación del Cliente B. Aunque sea "solo temporalmente", crea problemas de inventario difíciles de corregir.

---

### Facturación 3PL

P4 registra cada transacción para la facturación: almacenamiento por pallet o metro cúbico, recepciones, recolecciones, envíos y manejo especial.

**Para generar una factura de cliente:**
1. Ve a **3PL → Facturación**
2. Selecciona el cliente y el período de facturación
3. Revisa los cargos
4. Envía al cliente para su aprobación
5. Publica la factura

> 💡 **Consejo:** Revisa la facturación semanalmente, no solo al momento de facturar. Es mucho más fácil detectar y corregir errores cuando las transacciones acaban de ocurrir.

---

## Métricas de Desempeño

### ¿Por qué medir?

Lo que mides, puedes mejorar. Estos números te dicen qué tan bien está funcionando tu almacén — y dónde enfocar tu atención.

---

### Números clave a monitorear

**Recepción:**

| Qué medir | Meta | Cómo calcularlo |
|-----------|------|----------------|
| Tiempo desde el muelle hasta el stock | Menos de 4 horas | Tiempo recibido hasta ubicación confirmada |
| Exactitud de recepción | Más del 99% | Recepciones correctas ÷ total de recepciones |
| Captura de fecha de vencimiento | 100% | Obligatorio — cada artículo con vencimiento debe tener fecha |

**Recolección:**

| Qué medir | Meta | Cómo calcularlo |
|-----------|------|----------------|
| Recolecciones por hora | 60 o más | Total de recolecciones ÷ horas trabajadas |
| Exactitud de recolección | Más del 99.5% | Recolecciones correctas ÷ total de recolecciones |
| Tiempo de ciclo del pedido | Menos de 2 horas | Pedido liberado → empacado y listo |

**Envío:**

| Qué medir | Meta | Cómo calcularlo |
|-----------|------|----------------|
| Envío a tiempo | Más del 98% | Enviados a tiempo ÷ total de envíos |
| Exactitud de envío | Más del 99.5% | Envíos correctos ÷ total de envíos |

**Inventario:**

| Qué medir | Meta | Cómo calcularlo |
|-----------|------|----------------|
| Exactitud de inventario | Más del 99% | Espacios exactos ÷ total de espacios contados |
| Producto vencido | Menos del 0.5% | Valor vencido ÷ valor total del inventario |

---

### Dónde ver estos números en P4

- **Analítica → KPI** — Widgets de panel en tiempo real que puedes configurar para mostrar números en vivo
- **Analítica → Reportes** — Reportes detallados que puedes programar y enviar por correo electrónico
- **Despacho → Lista de Recolección** — Ver el estado de pedidos abiertos ahora mismo

---

## Capacitación y Mejora Continua

### Ruta de capacitación para nuevos empleados

| Semana | Enfoque |
|--------|---------|
| Semana 1 | Reglas de seguridad, recorrido del almacén, aprender los básicos de P4, cómo usar el dispositivo portátil |
| Semana 2 | Recepción y almacenamiento — práctica con un capacitador |
| Semana 3 | Recolección y empaque — recolecciones supervisadas con retroalimentación |
| Semana 4 | Envío y procesos especiales (devoluciones, conteos cíclicos) |

> 💡 **Consejo de capacitación:** La mejor manera de aprender es hacer las cosas con alguien observando. Comete errores mientras estás siendo supervisado — es mejor que cometerlos solo.

---

### Mejora continua

Cada mes, tómate 30 minutos para revisar:

1. **¿Qué salió mal?** Revisa errores, devoluciones causadas por errores del almacén, envíos tardíos
2. **¿Por qué salió mal?** ¿Fue capacitación? ¿Proceso? ¿Configuración del sistema?
3. **¿Qué cambiaremos?** Elige una cosa para corregir — no intentes arreglar todo a la vez
4. **¿Funcionó el cambio?** Revisa las métricas el mes siguiente

Las mejoras pequeñas y constantes se acumulan con el tiempo. Un almacén que aprende de sus errores mejora cada mes.

---

> ✅ **Recuerda:** Esta guía te da la base. Cada almacén es diferente. Habla con tu supervisor, haz preguntas, y cuando algo no se sienta bien — dilo. Los mejores almacenes tienen equipos que se comunican.
