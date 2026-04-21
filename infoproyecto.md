# AgroFlow






































# Tabla de Requerimientos del Sistema

## Requerimientos Funcionales

| ID | Requerimiento Funcional | Actor | Criterios de Aceptación |
|----|------------------------|-------|------------------------|
| RF-01 | El sistema debe permitir la comunicación directa entre agricultores y comerciantes para negociar y coordinar entregas. | Agricultor / Comerciante | El usuario puede enviar y recibir mensajes con otro usuario. Los mensajes se entregan en menos de 5 segundos. |
| RF-02 | El sistema debe mostrar la oferta y demanda de productos para que el comerciante evite depender de intermediarios. | Comerciante | Se visualizan productos disponibles con cantidades y precios actualizados. El comerciante puede contactar al productor directamente. |
| RF-03 | El sistema debe permitir al agricultor registrar la producción obtenida y las pérdidas de producto. | Agricultor | El agricultor puede ingresar datos de producción y pérdida por periodo. Los registros quedan almacenados y son comparables entre periodos. |
| RF-04 | El sistema debe permitir al comerciante comparar precios de un mismo producto entre distintos productores. | Comerciante | Se listan al menos dos productores con sus precios para el mismo producto. El comerciante puede ordenar los resultados por precio. |
| RF-05 | El sistema debe mostrar al productor los comercios interesados en comprar su producción. | Productor | El productor visualiza una lista de comerciantes con interés declarado en sus productos, incluyendo datos de contacto. |
| RF-06 | El sistema debe permitir al transportador planificar rutas de entrega para optimizar tiempo y costos. | Transportador | El transportador puede crear y editar rutas con múltiples paradas. El sistema muestra un resumen de la ruta. |
| RF-07 | El sistema debe mostrar al transportador los detalles de los envíos para planificar el transporte. | Transportador | Todos los datos del envío (origen, destino, volumen, peso, fecha) son visibles antes de aceptar el servicio. |
| RF-08 | El sistema debe permitir al transportador actualizar el estado de la entrega para informar a productores y comerciantes. | Transportador | El transportador puede cambiar el estado del envío y el cambio es visible para el productor y el comerciante de inmediato. |
| RF-09 | El sistema debe permitir al transportador registrar su disponibilidad para ofrecer sus servicios. | Transportador | El transportador puede indicar fechas y horarios disponibles. Su disponibilidad es visible para productores y comerciantes. |
| RF-10 | El sistema debe permitir al agricultor actualizar el estado de sus productos para mantener informados a los comerciantes. | Agricultor | El agricultor puede cambiar el estado de sus productos (disponible, agotado, en cosecha) y los comerciantes ven el cambio reflejado de inmediato. |
| RF-11 | El sistema debe permitir al comerciante buscar productos disponibles según sus necesidades. | Comerciante | El comerciante puede buscar por tipo de producto, región o productor y obtener resultados en menos de 3 segundos. |
| RF-12 | El sistema debe permitir al productor establecer precios para sus cosechas. | Productor | El productor puede ingresar y modificar el precio de cada producto. El precio actualizado es visible para los comerciantes de inmediato. |
| RF-13 | El sistema debe enviar alertas al comerciante cuando se publiquen nuevos productos disponibles. | Comerciante | El comerciante recibe una notificación en menos de 1 minuto tras la publicación de un nuevo producto. |
| RF-14 | El sistema debe permitir al productor actualizar la disponibilidad de sus productos para evitar vender productos agotados. | Productor | El productor puede marcar productos como agotados o disponibles. Los comerciantes no pueden realizar pedidos de productos marcados como agotados. |

---

## Requerimientos No Funcionales

| ID | Requerimiento No Funcional | Categoría | Criterios de Aceptación |
|----|---------------------------|-----------|------------------------|
| RNF-01 | El sistema debe estar disponible de forma continua para que agricultores, comerciantes y transportadores puedan operar en cualquier momento. | Disponibilidad | El tiempo de inactividad no supera 3.6 horas al mes medido en producción. |
| RNF-02 | Las respuestas del sistema deben ser rápidas para no interrumpir la negociación o coordinación entre usuarios. | Rendimiento | El 95% de las solicitudes responden en menos de 3 segundos bajo carga estándar. |
| RNF-03 | La información de precios, producción y datos de contacto debe estar protegida contra accesos no autorizados. | Seguridad | Toda comunicación usa HTTPS con TLS 1.2 o superior. Las contraseñas se almacenan con hash seguro (bcrypt o equivalente). |
| RNF-04 | El sistema debe ser usable desde dispositivos móviles, dado que los agricultores y transportadores operan en campo. | Usabilidad | La interfaz funciona correctamente en pantallas desde 360 px de ancho sin pérdida de funcionalidad. |
| RNF-05 | La interfaz debe ser comprensible para usuarios con bajo nivel de alfabetización digital. | Usabilidad | Pruebas con usuarios objetivo muestran una tasa de éxito mayor al 80% en tareas básicas sin capacitación previa. |
| RNF-06 | El sistema debe soportar el crecimiento en la cantidad de usuarios y productos registrados sin degradar el servicio. | Escalabilidad | Pruebas de carga con 500 usuarios simultáneos mantienen los tiempos de respuesta definidos en RNF-02. |
| RNF-07 | Los datos de producción, precios y entregas deben estar respaldados para evitar pérdidas de información. | Confiabilidad | Se realizan copias de seguridad automáticas diarias. La restauración de datos es posible en menos de 2 horas. |
| RNF-08 | El sistema debe cumplir con la normativa de protección de datos personales aplicable en Colombia. | Normativo | Se cuenta con política de privacidad publicada, consentimiento explícito del usuario y mecanismo para solicitar eliminación de datos (Ley 1581 de 2012). |
