---
title: 1. Presupuestación
category: Documentation
star: 9
sticky: 9
article: false
---

## Generar Proyecto de Constructora

El Proyecto de Constructora es una presupuestación sobre un determinado plan de obra que puede contener diversas "Fases", donde case estará compuesta por un determinado universo de productos.

Se trata de una unidad de gestión que agrupa un conjunto de entidades que le dan forma y describen un determinado Servicio.

El primer paso para la creación de un Proyecto de Constructora es ingresar en la ventana el nombre del cliente (Socio del negocio del cual hereda la dirección, lista de precio y el almacén), la fecha de inicio del servicio a realizar y seleccionar una categoría de Proyecto (y la unidad o departamento). En este paso solo se genera el evento (no se asignan recursos o productos). Además el sistema creará una línea de proyecto vacía para agilizar el proceso.

![Proyecto](/assets/img/docs/construction-management/com-image1.png)

### Generar Fase y Líneas de fase de proyecto

A partir del proyecto (cabezal) creado se generan las diferentes Fases del proyecto.

Las fases se dividen de acuerdo a los distintos segmentos (o universos) de productos que son determinadas características que poseen los productos .

En las fases se crean las líneas de proyecto listando los productos necesarios por cada fase con sus correspondientes cantidades.

Para lograr un circuito óptimo y eficiente de selección de productos en las líneas, es posible utilizar un proceso denominado "**Agregar Productos a Fase de Proyecto**". Este SB permite seleccionar los productos a través de parámetros para agilizar la selección y definición en las fases.

Cada producto tiene definido un determinado "Tipo de costo" (ejemplo: tipo de costo Herramientas).

Este tipo de costo define un costo para el producto en particular y ese costo multiplicado por la cantidad que se encuentre definido en la línea de la fase del proyecto será el que se muestre como importe costo de la línea del proyecto.

![Fase y línea](/assets/img/docs/construction-management/com-image2.png)

### Dimensionar Mano de Obra

En el producto es posible definir los parámetros de Unidad de duración y duración.

Determinando estas dos entidades y de acuerdo a la unidad de medida (y cantidad) es posible establecer la cantidad de mano de obra estimada que se necesitará por cada línea (y fase).

Esta función propone un cálculo eficiente (aproximado) de la cantidad de recursos (mano de obra) necesaria para un determinado proyecto).

## Reabastecimiento desde Línea de Proyecto

Desde el SB Reabastecimiento desde Línea de Proyecto es posible seleccionar el proyecto y la Fase (opcional). Al aceptar se desplegará el listado de todo lo que necesita alimentar ese proyecto (o Fase) para llevarse a cabo (los productos).

Luego, desde los parámetros es posible seleccionar si se desea generar una Orden de compra (para abastecer con los productos necesarios al proyecto/fase) o bien una requisición (una solicitud interna de compra).

![Reabastecimiento](/assets/img/docs/construction-management/com-image3.png)