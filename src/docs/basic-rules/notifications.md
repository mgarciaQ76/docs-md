---
title: Notificaciones
category: Documentation
star: 9
sticky: 9
article: false
---

## Definición de Notificaciones

Existen determinados eventos que generan notificaciones automáticas desde el ERP. 

Estas notificaciones pueden originarse por solicitudes entre diferentes usuarios del sistema, también por la ejecución de cálculo de morosidad con envío de estado de cuenta al cliente (envío de facturas o cuotas adeudadas), o bien desde reportes.

Cada evento que dispara un envío de información desde el sistema genera un registro de "cola de notificación". 

Este registro define el tipo de aplicación (ejemplo: correo electrónico) y la aplicación soportada (linkedin, facebook, etc).

### Tipos de Notificaciones

* Notificación desde Cálculo de Morosidad

  En la opción de Cálculo de Morosidad se generan las diferente entradas por deuda.

  Luego, el envío de estado de morosidad se realiza desde "Envío de Estado de cuenta por correo".

  Este proceso busca líneas de morosidad a enviar. Permite seleccionar por nivel de morosidad, por socio de negocio, por fecha. Y como parámetro se define el patrón de correo (de la organización correspondiente): generación de notificaciones desde línea de morosidad.

  ![Envio de Estado de cuenta por Correo](/assets/img/docs/basic-rules/bar-not-estado1.png)

* Notificación desde Solicitudes

  Generación de notificaciones desde solicitudes de trabajo (task, issues, request): es una entidad que puede vincularse a diferentes actores (usuarios) o documentos (proyecto, orden de venta, compra, facturas, etc.). Se puede generar desde cualquier documento.

  Se trata de comunicaciones entre los documentos del ERP. Tiene como objetivo una conexión total en la organización.

  Al crear solicitud deben llenarse campos obligatorios como organización, tipo de solicitud, asunto (título), resumen (texto sobre el origen de la solicitud), fecha de siguiente acción (o en la cual se espera una primera respuesta), tipo de vencimiento, prioridad, departamento y final de tiempo o fecha de vencido.

  Una vez guardada la solicitud, desde la opcipon de Recipiente de cola de notificación se podrán visualizar las diferentes solicitudes creadas y su estado.

 ![Solicitud](/assets/img/docs/basic-rules/bar-not-solicitud1.png)

* Notificación desde Proyectos

  Es posible vincular una solicitud a un proyecto (así como a otras entidades). O bien, en sentido contrario, es posible generar una solicitud que posteriormente será origen de un proyecto (en ambos casos quedarán vinculados). 

  La ventaja de generar las Solicitudes desde un Proyecto, Fase o Tarea es que tomará del contexto toda la información que necesite, como Proyecto, Cliente, etc.

  Desde la ventana Proyecto se podrá visualizar todas las Solicitudes relacionadas, tanto desde la Pestaña de Solicitudes correspondiente como desde la Barra de herramientas (Ver todas las solicitudes).

  El objetivo de la vinculación entre proyecto y solicitud responde a la necesidad de ligar las diferentes tareas y requerimientos que se vayan generando a diferentes usuarios, y que tengan relación con un determinado proyecto.

   ![Proyecto](/assets/img/docs/basic-rules/bar-not-proyecto1.png)

* Notificación desde Reportes

  Desde las diferentes entidades del ERP existe una opción en la barra de comandos denominada "Informes". Desde allí es posible generar un reporte con aquella información que se esté visualizando en pantalla, seleccionar una extensión (ejemplo, PDF, HTML,, excel) y luego exportarlo. A su vez, esta exportación es posible enviarla por mail desde el sistema. Esto genera un registro de cola de notificación).

   ![Informe](/assets/img/docs/basic-rules/bar-not-report3.png)

    ![Reporte](/assets/img/docs/basic-rules/bar-not-report4.png)

### Configuración de Notificaciones por Usuario

En la opción de Solicitudes, pestaña Aviso de Actualización puede observarse a aquellos usuarios que serán notificados por cambios en una determinada solicitud (ya sea por autor, por asignado, o por seguidor, y las diferentes modificaciones de la solicitud).

Desde la solicitud será posible la carga de horas por usuario (timesheet).

### Plantilla de Correo

En la opción de Plantilla de notificación es posible configurar templates por tipo de plantilla (ejemplo: solicitudes, proyectos).

 ![Plantilla de Correo](/assets/img/docs/basic-rules/bar-not-plantilla1.png)

### Plantilla de Correo por Evento (¿Qué se envía?)

Permite configurar diferentes formatos o templates por cada evento de aquella información que deseamos enviar por cada notificación.
Motor de Templates para reemplazo de campos en template

El template admite poder referenciar campos locales y referentes en otras tablas, se debe ingresar como texto en el template el nombre de la columna entre @ (arrobas), a su vez podrá referenciarse información desde otra tabla indicando el nombre de la tabla, punto, el nombre del campo.

 ![Plantilla de Correo por Evento](/assets/img/docs/basic-rules/bar-not-event1.png)

### Cuando se genera cada Notificación?

Al crearse un evento (al grabar solicitud por ejemplo) dentro de la aplicación que aplique un envío de información (una solicitud o bien, un envío de estado de cuenta de educación), se genera un registro de cola de notificación. Luego, un programador de procesos arma la cola de notificación (cada cinco minutos corre el proceso automático). Se limita el envío a 20 notificaciones por lote.

Solicitudes automáticas: se está avanzando en la automatización de solicitudes ante escenarios específicos que se van generando en el ERP. Puede ser el caso de una factura recibida que no cuadre su importe con la orden. En este caso se cerrará la orden y se emitirá una solicitud (automática) para pedir la generación de nota de crédito (esto generará notificaciones por correo).

### A quién se envía notificación?

Es posible confirmar quienes son los destinatarios de una notificación desde la opción de Solicitudes, pestaña Aviso de Actualización (usuarios que serán notificados) por cambios en determinada solicitud por ejemplo.

Cada Solicitud envía **notificaciones** de sus actualizaciones a los usuarios definidos como:

* Asignado A
* Creado Por
* Departamento
* Aviso de Actualización

Además de los usuarios vinculados, dentro de cada Solicitud se podrá agregar diferentes usuarios para que les llegue vía correo electrónico las **notificaciones** por actualización de las mismas, independientemente de los demás criterios. Para ello simplemente se deberá navegar a la pestaña “Aviso de Actualización” y agregar manualmente el o los usuarios a recibir notificaciones.

 ![Aviso de Actualización](/assets/img/docs/basic-rules/bar-not-act1.png)

### Proceso de Envío de Cola de Notificaciones

El registro de cola de notificación se genera con un destinatario (es uno a uno). El estado de procesado = NO cambia a "SI" cuando se realiza el envío de la notificación. En el caso de fallar o emitir error por envío, queda configurado como Procesado = NO (descripción del error) y Activo = no para que no ingrese en el siguiente lote de envío.

### Cola de Notificación

Cuando se dispara una notificación desde el ERP, al generarse registro de cola de notificación, se graba como procesado = No (no enviado) y con el check de Activo = SI

El envío de notificación tiene diferentes funcionalidades: se puede generar desde

* El usuario
* La organización
* La compañia

From Account name: desde donde se origina la notificación.

 ![Cola de Notificación](/assets/img/docs/basic-rules/bar-not-notification1.png)

### Recipientes de Cola de Notificación

Es un registro de notificaciones generados dentro del sistema y con sus diferentes destinatarios. 

Es como una auditoría o historial de envíos de notificación con sus correspondientes estados y descripción de error (en el caso de no haber sido enviados).

 ![Recipiente de Cola de Notificación](/assets/img/docs/basic-rules/bar-not-recipient1.png)