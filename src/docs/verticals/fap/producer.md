---
title: Productor (Agricultor)
category: Documentation
star: 9
sticky: 9
article: false
---

En esta ocasión **Solop ERP** pretende ofrecerle una guía fácil para la definición de un productor en Solop ERP, es importante seguir paso a paso cada procedimiento, de ello dependerá el éxito de los registros resultantes.

- Registro de Productor
  - Pestaña Localización del Productor
  - Pestaña Contacto
  - Pestaña Finca

## Registro de Productor

Ubique y seleccione en el menú de Solop ERP, la carpeta **Gestión de Asistencia Técnica Agricola**, luego seleccione la carpeta **Configuración de Asistencia Técnica**, por último seleccione la carpeta **Configuración de Productor**. Finalmente, seleccione la ventana **Productor**.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image161.png)

Imagen 1. Menú de Solop ERP

Podrá visualizar la ventana **Productor**, con los diferentes registros de productores que contiene Solop ERP.

En esta ventana se registran los datos principales que la empresa requiere del productor. Cada uno de los campos con el símbolo (\*) son obligatorios para el registro.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image162.png)

Imagen 2. Ventana Productor

Seleccione el icono **Registro Nuevo**, ubicado en la barra de herramientas de Solop ERP, para registrar un nuevo productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image163.png)

Imagen 3. Icono Registro Nuevo de la Ventana Productor

Seleccione en el campo **Organización**, la organización para la cual se encuentra realizando el registro del productor.

La organización le permite definir la entidad legal ó una sub-unidad a la cual pertenece el productor, si la organización es (\*), este estará disponible para todas las organizaciones al procesar documentos y transacciones, pero si por el contrario, ha seleccionado una organización diferente, este registro únicamente estará disponible para la organización seleccionada.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image164.png)

Imagen 4. Campo Organización de la Ventana Productor

Introduzca en el campo **Código**, el código correspondiente al registro del productor que se encuentra realizando.

El código es un dato único e irrepetible que protege la entrada de los registros, evitando la duplicidad de los mismos, generalmente se refiere al número de identificación que acredite la identidad de una persona natural una entidad jurídica, por ejemplo, una cédula de identidad o un RIF.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image165.png)

Imagen 5. Campo Código de la Ventana Productor

Podrá visualizar el número de identificación autogenerado a partir del campo Código en el campo **Número de Identificación**.

El número de identificación se refiere al número que acredita la identidad de una persona natural una entidad jurídica, por ejemplo, una cédula de identidad o un RIF, este campo mantiene incidencia en la generación de documentos fiscales como facturas, retenciones y comprobantes ARC.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image166.png)

Imagen 6. Campo Número Identificación de la Ventana Productor

Seleccione en el campo **Saludo**, el saludo a utilizar en la correspondencia enviada al productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image167.png)

Imagen 7. Campo Saludo de la Ventana Productor

Introduzca el nombre del productor en el campo **Nombre**.

El nombre se refiere a la razón social, siendo esta el nombre ó la denominación con la que está registrado en los documentos legales, el nombre es utilizado a nivel administrativo, formal y jurídico.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image168.png)

Imagen 8. Campo Nombre

Introduzca el nombre 2 del productor en el campo **Nombre 2**.

El nombre 2 varía su uso dependiendo de la naturaleza del productor, generalmente se utiliza para colocar la denominación comercial.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image169.png)

Imagen 9. Campo Nombre 2 de la Ventana Productor

Introduzca una breve descripción referente al productor en el campo **Descripción**.

La descripción no es un campo obligatorio,sin embargo, le permite dejar descripciones o notas de interés para el registro.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image170.png)

Imagen 10. Campo Descripción

Seleccione el estado de crédito del productor en el campo **Estado de Crédito**.

El estado del crédito no es un campo obligatorio, sin embargo, le permite definir el comportamiento para la gestión del crédito del productor, actúa conjuntamente con el campo Saldo Actual, este puede variar entre las siguiente opciones dependiendo de las necesidades:

Sin Verificación de Crédito: Establecido de forma manual, omite la evaluación para los productores a los que no se evalúa el crédito, equivalente a Sin límite de Crédito.

Crédito Correcto: Activa la gestión de crédito por estar dentro del límite de cŕedito.

Crédito Verificación: Es establecido de forma automática por Solop ERP al evaluar el crédito, cuando el saldo actual está por encima del % de crédito en verificación (por defecto es 90%) del límite de crédito pero no alcanza el 100%.

Crédito Retenido: Es establecido de forma automática por Solop ERP al evaluar el crédito, cuando el saldo actual está por encima del límite de crédito, bloqueando la posibilidad de completar ordenes de ventas, completar facturas y emitir entregas.

Crédito Detenido: Establecido de forma manual, bloqueando la posibilidad de completar ordenes de ventas, completar facturas y emitir entregas.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image171.png)

Imagen 11. Campo Estado de Crédito

Podrá visualizar el saldo actual que posee el productor en el campo \*\*Saldo Actual.

El saldo actual es un campo solo lectura, actualizado de forma automática, aumentando o disminuyendo al emitir cuentas por cobrar o cuentas por pagar, controlando el estado de crédito.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image172.png)

Imagen 12. Campo Saldo Actual

Seleccione el checklist **Exento de Impuesto en Venta**.

Exento de Impuesto de Venta, no es un campo obligatorio, por defecto está establecido en falso, permite la omisión de impuestos al generar ordenes de ventas, es decir si un producto es gravado, hará una excepción para este productor, emitiendo la orden de venta con el producto en cuestión con impuesto (0%).

![Campo](/assets/img/docs/assistance-management/atm-assistance-image173.png)

Imagen 13. Campo Exento de Impuesto en Venta

Seleccione el checklist **Exento de Impuesto en Compra**, para definir al productor como exento de impuesto.

Exento de Impuesto de Compra, no es un campo obligatorio, por defecto está establecido en falso, permite la omisión de impuestos al generar ordenes de compras, es decir si un producto es gravado, hará una excepción para este productor, emitiendo la orden de compra con el producto en cuestión con impuesto (0%).

![Campo](/assets/img/docs/assistance-management/atm-assistance-image174.png)

Imagen 14. Campo Exento de Impuesto en Compra

Seleccione el grupo de socio del negocio en el campo **Grupo de Socio del Negocio**.

El grupo de socio del negocio, permite categorizar sus productores de una forma específica, lo cual es eficiente a la hora de emitir asientos contables y reportes, para entenderlo mejor veamos el siguiente ejemplo:

![Campo](/assets/img/docs/assistance-management/atm-assistance-image175.png)

Imagen 15. Campo Grupo de Socio del Negocio

Por defecto se encuentran tildados los checklist **Productor**, **Proveedor** y **Cliente**, considerando que un productor puede ser proveedor o cliente de la organización en la cual se encuentra realizando el registro.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image176.png)

Imagen 16. Checklist Productor, Proveedor y Cliente

Note

Recuerde guardar el registro de los campos de la pestaña **Productor**, antes de seleccionar cualquier otra pestaña de la ventana **Productor**. El registro se guarda seleccionando el icono **Guardar Cambios**, ubicado en la barra de herramientas de Solop ERP.

### Pestaña Localización del Productor

La localización de un productor es muy importante por diferentes motivos, ya que las transacciones de ventas serán realizadas al mismo, en esta pestaña se deben registrar con exactitud los datos de la dirección del mismo.

Seleccione la pestaña **Localización** que se encuentra ubicada del lado izquierdo de la ventana productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image177.png)

Imagen 17. Pestaña Localización

Introduzca en el campo **Localización / Dirección**, la dirección de localización del productor con ayuda del identificador.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image178.png)

Imagen 18. Campo Localización / Dirección

Seleccione en el campo **País**, el país donde se encuentra domiciliado el productor que esta registrando.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image179.png)

Imagen 19. Campo País

Seleccione en el campo **Estado**, el estado donde se encuentra domiciliado el productor que esta registrando.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image180.png)

Imagen 20. Campo Estado

Seleccione en el campo **Ciudad**, la ciudad donde se encuentra domiciliado el productor que esta registrando.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image181.png)

Imagen 21. Campo Ciudad

Introduzca la dirección detallada del productor en el campo **Dirección 1** y seleccione la opción **OK**.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image182.png)

Imagen 22. Campo Dirección 1

Introduzca en el campo **Teléfono**, el número de teléfono local para contactar al productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image183.png)

Imagen 23. Campo Teléfono

Introduzca en el campo **Teléfono Móvil**, el número de teléfono móvil para contactar al productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image184.png)

Imagen 24. Campo Teléfono Móvil

Introduzca en el campo **Fax**, el fax para contactar al productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image185.png)

Imagen 25. Campo Fax

Introduzca en el campo **ISDN**, el ISDN para contactar al productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image186.png)

Imagen 26. ISDN

Podrá apreciar tildados los checklist **Dirección Entregar-A**, **Dirección Facturar-A**, **Dirección Pagar-Desde** y **Dirección Remitir-A**, indicando cada uno de ellos un comportamiento diferente.

El checklist **Dirección Entregar-A** establece la localización ingresada como la dirección para embarcar los bienes.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image187.png)

Imagen 27. Campo Dirección Entregar-A

El checklist **Dirección Facturar-A** establece la localización ingresada como la dirección para facturar.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image188.png)

Imagen 28. Campo Dirección Facturar-A

El checklist **Dirección Pagar-Desde** establece la localización ingresada como la dirección desde donde paga las facturas el productor y donde son enviadas las cartas de morosidad.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image189.png)

Imagen 29. Campo Dirección Pagar-Desde

El checklist **Dirección Remitir-A** establece la localización ingresada como la dirección para el envío de los pagos.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image190.png)

Imagen 30. Dirección Remitir-A

Seleccione en el campo **Región de Ventas**, la región o área de ventas en la que se encuentra localizado el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image191.png)

Imagen 31. Campo Región de Ventas

Note

Para conocer más sobre las regiones de ventas que puede tener una compañía u organización, visite el documento Registro de Región de Ventas, elaborado por ERPyA.

Warning

Recuerde guardar el registro de los campos cada vez que se vaya a posicionar en una pestaña de la ventana productor.

### Pestaña Contacto

En esta pestaña se registran todos los datos de contacto que se posea el productor.

Seleccione la pestaña **Contacto** que se encuentra ubicada del lado izquierdo de la ventana productor, para proceder a llenar los campos necesarios.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image192.png)

Imagen 32. Pestaña Contacto

Warning

El contacto (Usuario) permite registrar las diferentes personas de contacto que tiene la empresa con el productor que esta registrando. Un ejemplo de esta pestaña puede ser, un jefe o persona de contacto por departamento para que a la hora de alguna venta de productos o servicios al productor, se contacte a la persona correspondiente.

Introduzca en el campo **Nombre**, el nombre completo de la persona de contacto con el productor que esta registrando.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image193.png)

Imagen 33. Nombre de Contacto

Introduzca en el campo **Descripción**, una breve descripción de la persona de contacto con el productor que esta registrando.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image194.png)

Imagen 34. Campo Descripción

Introduzca en el campo **Comentarios**, los comentarios o información adicional sobre el registro de la persona de contacto con el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image195.png)

Imagen 35. Campo Comentarios

El checklist **Activo**, indica que el registro se encuentra activo en el sistema.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image196.png)

Imagen 36. Checklist Activo

Introduzca en el campo **Email**, el correo electrónico de la persona de contacto con el productor para las transacciones entre las empresas.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image197.png)

Imagen 37. Campo Email

Introduzca en el campo **Contraseña**, la contraseña de acceso del usuario.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image198.png)

Imagen 38. Campo Contraseña

Seleccione en el campo **Saludo**, la forma de saludar a la persona de contacto con el productor en los documentos a ser enviados.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image199.png)

Imagen 39. Campo Saludo

Seleccione en el campo \*\*Dirección del Socio del Negocio, la dirección de ubicación de la persona de contacto con el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image200.png)

Imagen 40. Campo Dirección del Socio del Negocio

Introduzca en el campo **Título**, el nombre del productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image201.png)

Imagen 41. Campo Título

Seleccione en el campo **Cumpleaños**, la fecha de nacimiento de la persona de contacto con el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image202.png)

Imagen 42. Campo Cumpleaños

Introduzca en el campo **Teléfono**, el teléfono para localizar a la persona de contacto con el productor para las transacciones entre las empresas.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image203.png)

Imagen 43. Campo Teléfono de Contacto

Introduzca en el campo **Teléfono Móvil**, el teléfono móvil para localizar a la persona de contacto con el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image204.png)

Imagen 44. Campo Teléfono Móvil

Introduzca en el campo **Fax**, el fax de contacto del productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image205.png)

Imagen 45. Campo Fax

Seleccione en el campo **Tipo de Notificación**, la forma de enviar notificaciones a la persona de contacto con el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image206.png)

Imagen 46. Campo Tipo de Notificación

Seleccione en el campo **Posición**, la posición de trabajo de la persona de contacto con el productor.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image207.png)

Imagen 47. Campo Posición

Podrá apreciar el checklist **Acceso Total Socio del Negocio**, que al estar tildado indica que la persona de contacto con el productor posee acceso total a su rol.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image208.png)

Imagen 48. Campo Acceso Total Socio del Negocio

Warning

Recuerde guardar el registro de los campos cada vez que se vaya a posicionar en una pestaña de la ventana productor.

### Pestaña Finca

Al seleccionar el productor en el registro de una finca, se carga de manera automática en la pestaña **Finca** de la ventana **Productor**, los datos registrados en la pestaña **Finca**, de la ventana **Finca**.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image209.png)

Imagen 49. Pestaña Finca de la Ventana Productor

Si el registro de la finca contiene información en la pestaña **Lote de Finca**, esta se carga de manera automática a la pestaña **Lote** de la ventana **Productor**.

![Campo](/assets/img/docs/assistance-management/atm-assistance-image210.png)

Imagen 50. Pestaña Lote de Finca de la Ventana Productor
