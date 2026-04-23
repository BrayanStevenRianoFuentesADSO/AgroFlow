# AgroFlow
## *Visión*


AgroFlow nace de una realidad que afecta a miles de 
familias en el campo: los agricultores pierden sus 
cosechas por no encontrar compradores a tiempo, los 
comerciantes asumen costos elevados por culpa de cadenas 
de intermediarios innecesarias, y el transporte agrícola 
opera de manera desorganizada, generando pérdidas 
económicas y desperdicio de alimentos que podrían 
evitarse.

Nuestra visión es construir el ecosistema digital más 
completo y accesible para el agro, donde productores, 
comerciantes y transportadores se conecten de forma 
directa, transparente y eficiente, eliminando las 
barreras que históricamente han fragmentado la cadena de 
valor agrícola.

A través de AgroFlow, los agricultores podrán registrar 
sus cosechas en tiempo real, acceder a una red activa de 
compradores y negociar precios justos sin depender de 
terceros que se quedan con la mayor parte de sus 
ganancias. Los comerciantes, por su parte, podrán 
publicar sus necesidades de abastecimiento, comparar 
ofertas y planificar sus compras con anticipación, 
reduciendo costos y garantizando la calidad de los 
productos que adquieren.

El tercer pilar de AgroFlow es la red de transporte 
colaborativa, un sistema inteligente que coordina rutas, 
optimiza cargas y conecta a los transportadores con 
quienes realmente los necesitan, reduciendo tiempos de 
entrega, disminuyendo el costo logístico y minimizando 
el impacto ambiental del transporte agrícola.
Creemos en un campo más justo, más tecnológico y más 
conectado. AgroFlow no es solo una plataforma; es una 
apuesta por la transformación del sector agrícola desde 
sus raíces, poniendo la tecnología al servicio de 
quienes producen los alimentos que sostienen a toda una 
sociedad.


![Imagen_agricola](https://radionacional-v3.s3.amazonaws.com/s3fs-public/node/article/field_image/Campesinofinagro%20%281%29.jpg)


### **Definicion de Stakeholders:**

***Agricultores:*** 
 Son los encargados de la producción de la materia comerciada *(como frutas, verduras , vegetales, carne, etc)*. Se enfrentan a la problemática del desperdicio de productos por falta de conexión directa entre los
pequeños productores y distintos mercados locales.

![Agricultores](https://www.univision.com/_next/image?url=https%3A%2F%2Fst1.uvnimg.com%2F4c%2F66%2F07016be249a1a4272b751ec110cb%2Fgettyimages-471373404.jpg&w=1280&q=75)

***Transportadores / Intermediarios:***  
Son los encargados de intermediar entre los agricultores y los mercados locales, esto al transportar los productos que ofrecer los agricultores. Los intermediarios se enfrentan a los precios altos del transporte de la materia debido a una combinación de altos costos operativos, poder de mercado para fijar precios y la necesidad de cubrir riesgos en una cadena de suministro a menudo ineficiente.

![Transportadores](https://cdn.agroempresario.com/images/posts/f45d9b163f01291c0b0837a24239f8c06405288f03c62a8b_840.jpg)

***Mercados Locales:*** Son los encargados de conectar la producción con el hogar. Su función principal es el abastecimiento de alimentos frescos y productos de primera necesidad en un área geográfica delimitada, como un barrio, pueblo o ciudad. Se enfrentan a problemáticas como: Altos Precios de Productos e Insumos: Esto al comprar a los Intermediarios y administrar estos mercados; Informalidad de estos mercados: Usualmente son plazas, mercados municipales,ferias campesinas, etc. ; Pérdida de Alimentos: Debido a poco manejo de medidas alimenticias, causadas por el clima, lugar de trabajo y demás.

![Mercados Locales](https://muniguatealfrente.com/wp-content/uploads/WhatsApp-Image-2025-07-10-at-10.38.40-AM-3.jpeg)











































































# **Épicas:**

## *Épica 1: Agricultores*
### Gestión y comercialización de productos agrícolas por parte del agricultor:

***Descripción:***
Como plataforma, se quiere lograr que los agricultores gestionen su producción y comercialicen directamente sus productos con los comerciantes, facilitando la comunicación, el control de inventario y la definición de las condiciones de venta.

***Objetivos / Tareas:***
- Incrementar las oportunidades de venta del agricultor

- Reducir la dependencia de intermediarios

- Mejorar la gestión de producción y pérdidas

- Asegurar información actualizada para los compradores

- Criterios de Aceptación:

- El agricultor puede registrar y actualizar su producción

- El agricultor puede publicar productos disponibles

- El agricultor puede definir precios

- El agricultor puede ver interesados en sus productos

- El agricultor puede comunicarse con comerciantes

- La información de productos se mantiene actualizada

  

***Historias de usuario asociadas:***

- Como agricultor, quiero tener comunicación directa con los comerciantes para negociar y coordinar entregas

- Como agricultor, quiero conocer comercios interesados en mi producción para ampliar mis ventas

- Como agricultor, quiero llevar un conteo de producción y pérdidas para analizar resultados

- Como agricultor, quiero actualizar el estado de mis productos para informar a los comerciantes

- Como agricultor, quiero actualizar la disponibilidad de mis productos para evitar inconsistencias

- Como agricultor, quiero establecer precios para mis cosechas

<br>
<br>


# *Épica 2: Transportadores / Intermediarios*
## Coordinación inteligente de la red de transporte agrícola en AgroFlow

***Descripción***

- Esta épica agrupa todas las funcionalidades necesarias para que los transportadores puedan integrarse activamente dentro de la plataforma AgroFlow. 
- Busca que el transporte deje de ser un proceso desorganizado y costoso, convirtiéndose en una red colaborativa.
- Los transportadores podrán gestionar su disponibilidad, planificar rutas eficientes, acceder a detalles de envíos y mantener informados en tiempo real a agricultores y comerciantes.



***Objetivos / Tareas***

*Objetivo 1 — Incorporación del transportador a la plataforma*

- Crear formulario de registro de disponibilidad del transportador

- Definir campos clave: fechas disponibles, zona de cobertura, tipo y capacidad del vehículo

- Desarrollar endpoint POST /transportadores/disponibilidad

- Permitir edición y actualización de disponibilidad en cualquier momento
  

*Objetivo 2 — Acceso a información de envíos*

- Desarrollar vista de detalle de cada solicitud de envío

- Mostrar información de origen, destino, tipo de producto, peso y fecha requerida

- Filtrar envíos por zona geográfica y tipo de carga

- Desarrollar endpoint GET /envios/:id


*Objetivo 3 — Planificación de rutas*

- Implementar módulo de planificación de rutas con múltiples paradas

- Calcular distancia, tiempo estimado y costo aproximado por ruta

- Permitir al transportador aceptar o rechazar solicitudes según su ruta planificada

- Objetivo 4 — Seguimiento y actualización de entregas

- Crear sistema de estados: Pendiente, En camino, Entregado

- Notificar automáticamente al agricultor y comerciante en cada cambio de estado

- Registrar historial de entregas por transportador

- Desarrollar endpoint PATCH /envios/:id/estado

  

***Criterios de Aceptación:***

- CA-01: El transportador puede registrar su disponibilidad con fecha, zona y tipo de vehículo

- CA-02: El transportador puede ver el detalle completo de un envío antes de aceptarlo

- CA-03: El sistema muestra una ruta planificada con tiempo y costo estimado

- CA-04: El transportador puede actualizar el estado del envío en tiempo real

- CA-05: Agricultores y comerciantes reciben notificación ante cada cambio de estado

- CA-06: El transportador solo ve envíos compatibles con su zona y capacidad

- CA-07: El historial de entregas queda registrado en el perfil del transportador

  

## ***Historias de Usuario Asociadas:***


*HU-T01 — Registro de disponibilidad:*

**Descripción:** Como transportador, quiero registrar mi disponibilidad para ofrecer mis servicios de transporte
**Sprint sugerido:** 1
**Prioridad:** Alta


HU-T02 — Ver detalles del envío

**Descripción:** Como transportador, quiero ver detalles de los envíos para planificar correctamente el transporte
**Sprint sugerido:** 1
**Prioridad:** Alta


HU-T03 — Planificación de rutas

**Descripción:** Como transportador, quiero planificar rutas de entrega para optimizar tiempo y costos
**Sprint sugerido:** 2
**Prioridad:** Alta


HU-T04 — Actualización de estado de entrega

**Descripción:** Como transportador, quiero actualizar el estado de la entrega para informar a productores y comerciantes
**Sprint sugerido:** 2
**Prioridad:** Alta

<br>
<br>


# *Épica 3: Comerciantes / Mercados Locales:*

## Participación y gestión de compras en mercados locales por parte del comerciante

***Descripción:***
Como plataforma, se quiere lograr que los comerciantes participen activamente en los mercados locales, pudiendo buscar, analizar y adquirir productos directamente de los agricultores, facilitando la comparación de opciones, el acceso a información del mercado y la comunicación directa para optimizar sus decisiones de compra.


***Objetivos / Tareas:***

- Incrementar las oportunidades de compra directa del comerciante

- Reducir la dependencia de intermediarios

- Mejorar la toma de decisiones mediante información del mercado

- Asegurar acceso a información actualizada de productos disponibles

- Criterios de Aceptación:

- El comerciante puede buscar productos disponibles

- El comerciante puede comparar precios entre productores

- El comerciante puede consultar información de oferta y demanda

- El comerciante puede recibir alertas de nuevos productos disponibles

- El comerciante puede comunicarse directamente con agricultores

- La información de productos se mantiene actualizada


  

## ***Historias de Usuario Asociadas:***

- Como comerciante, quiero buscar productos disponibles para comprar según mis necesidades

- Como comerciante, quiero comparar precios entre distintos productores para elegir la mejor opción

- Como comerciante, quiero conocer la oferta y demanda de los productos para evitar precios elevados

- Como comerciante, quiero recibir alertas de nuevos productos para aprovechar oportunidades de compra

- Como comerciante, quiero comunicarme directamente con los agricultores para negociar condiciones de compra

