---
title: "Centros educativos"
date: 2022-2-8
weight: 6
description: >
  
tags: [proyectos]
---

{{% pageinfo %}}
**Descripción**: proyecto de aplicación usando el CMS Wagtail
{{% /pageinfo %}}


## Objetivo
Añadir una aplicación de centros educativos al proyecto anterior.

La aplicación tendrá una página principal (tipo índice) que mostrará los datos de todos los centros o una selección que pueda hacer el usuario 

## Datos 
https://opendata.aragon.es/datos/catalogo/dataset/educacion-y-cultura

En concreto usaremos el ```json``` de los centros educativos de Aragón: https://opendata.aragon.es/GA_OD_Core/download?view_id=167&formato=json

## Modelo de Centros
Datos que interesan. Los sacaremos del json y los cargaremos de forma automática en la aplicación.

* Código del centro (idcentrorc)
* Nombre del centro
* Tipo de centro
* Naturaleza (público o privado)
* Localidad
* Dirección
* Código postal
* Coordenadas (longitud y latitud)
  
## Páginas
La aplicación tendrá:
* Una página con un tabla con el listado paginado y la posibilidad de buscar por nombre del centro o localidad.
* Una página con el mapa de todos los centros

## Admin
* list_view tabulado con datos de nombre, código, naturaleza y localidad
* búsqueda por nombre y localidad
* fitro por tipo de centro y naturaleza.