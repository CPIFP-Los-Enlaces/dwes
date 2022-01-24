---
title: "Aplicación películas"
date: 2021-10-21T10:36:54+02:00
weight: 85
description: >
  Aplicación de películas
tags: []
---

{{% pageinfo %}}
Crear una aplicación de películas con la informaciń del siguiente archivo json. Es la lista de las películas más vistas de [imdb.com](https://www.imdb.com/chart/top/?ref_=nv_mv_250_6).
{{% /pageinfo %}}


* [Películas](listapelis.json)

## Ayudas

### Ejecutar script de django
```bash
python manage.py shell < url_script.py
```

### slugify
* https://docs.djangoproject.com/en/4.0/ref/utils/#django.utils.text.slugify
* para rellenar campos **models.SlugField()**
* Ejemplo: https://learndjango.com/tutorials/django-slug-tutorial



