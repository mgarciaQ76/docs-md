---
title: Docker
icon: docker
category: Descarga
star: 9
sticky: 9
tag:
  - Docker
  - Docker Hub
article: false
---

[Docker](https://www.docker.com/) es una forma sencilla de arrancar un despliegue de aplicación, funciona bajo un esquema de contenedores que permiten reutilizar recursos y librerías de un sistema operativo. 

## Imágenes Oficiales

Todas las imágenes oficiales de [Solop ERP](https://solopsoftware.com/) se encuentran [aquí](https://hub.docker.com/u/erpya). Invertimos muchas horas y recursos en hacer que nuestra infraestructura sea de clase mundial. No vamos por el camino fácil, en su lugar vamos por el camino correcto.

Puedes ver los enlaces a nuestras imágenes en la siguiente lista

- [Solop ERP ZK UI](https://hub.docker.com/r/erpya/adempiere-zk-ui)
- [Solop ERP Vue UI](https://hub.docker.com/r/erpya/adempiere-vue)
- [Solop ERP gRPC Server](https://hub.docker.com/r/erpya/adempiere-grpc-server)
- [Solop ERP Proxy Server](https://hub.docker.com/r/erpya/proxy-adempiere-api)
- [Solop ERP Backend](https://hub.docker.com/r/erpya/backend)
- [Solop ERP Middleware](https://hub.docker.com/r/erpya/adempiere-middleware)
- [Microservicio para Punto de Ventas](https://hub.docker.com/r/erpya/ms-point-of-sales-rs)

## Despliegue para Demo (Docker Compose)

Si solo quieres ver nuestros productos puedes hacer un despliegue local de manera rápida con [Docker Compose](https://docs.docker.com/compose/).

Para hacer el despliegue local puedes descargar [este](https://github.com/erpya/adempiere-all-services) repositorio y seguir las siguientes instrucciones.


### Requerimientos

Sólo necesitas instalar [git](https://git-scm.com/downloads) y [Docker Compose v2.16.0 o superior](https://docs.docker.com/compose/install/linux/)

### Clona el repositorio

```
git clone https://github.com/adempiere/adempiere-all-services
```

### Ubica el directorio clonado

```
cd adempiere-all-services
```
### Haz una copia de la plantilla de despliegue

```
cp env_template .env
```

### Levanta el servicio

```
docker compose up
```

![Despliegue](https://github.com/erpya/adempiere-all-services/blob/main/docs/ADempiere_All_Services_Vue.gif)