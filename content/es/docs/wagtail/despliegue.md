---
title: "Despliegue"
date: 2021-10-21T10:36:54+02:00
weight: 90
description: >
  Servidor en producción
tags: []
---

{{% pageinfo %}}
 * https://docs.wagtail.org/en/stable/advanced_topics/deploying.html
 * https://docs.djangoproject.com/en/stable/howto/deployment/
 * https://docs.wagtail.org/en/stable/advanced_topics/performance.html

{{% /pageinfo %}}


## Requisitos
* Postgresql
* Elasticsearch
* Redis
* Varnish ? 
* Gunicorn


### Gunicorn 
* https://docs.gunicorn.org/en/latest/deploy.html
  
### Tutoriales
* https://www.digitalocean.com/community/tutorials/how-to-set-up-django-with-postgres-nginx-and-gunicorn-on-ubuntu-20-04-es
* https://esdjango.com/configuracion-de-gunicorn-y-nginx-para-django.html

* https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-elasticsearch-on-ubuntu-20-04-es