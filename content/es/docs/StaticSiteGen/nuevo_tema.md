---
title: "Crear un tema"
date: 2017-01-05
weight: 18
description: 

---

{{% pageinfo %}}
Creación de un nuevo tema

**Documentación:**  
* https://gohugo.io/commands/hugo_new_theme
* https://gohugo.io/templates/
* https://gohugo.io/hugo-modules/theme-components/
{{% /pageinfo %}}

## Creación de un nuevo tema

```bash
$ hugo new theme <THEME_NAME>
$ hugo new theme basico

themes/basico/
├── LICENSE
├── archetypes
│ └── default.md
├── layouts
│ ├── 404.html
│ ├── _default
│ │ ├── baseof.html
│ │ ├── list.html
│ │ └── single.html
│ ├── index.html
│ └── partials
│
├── footer.html
│
├── head.html
│
└── header.html
├── static
│ ├── css
│ └── js
└── theme.toml
```


## Content blocks y partials

### themes/basico/layouts/_default/baseof.html

```go-html-template
<!DOCTYPE html>
<html>
  {{- partial "head.html" . -}}
  <body>
  {{- partial "header.html" . -}}
    <div id=​ "content"​ >
    {{- block "main" . }}{{- end }}
    </div>
  {{- partial "footer.html" . -}}
  </body>
</html>

```

### themes/basico/layouts/partials/head.html

```go-html-template
<head>
<meta charset=​ "utf-8"​ >
<meta name=​ "viewport"​ content=​ "width=device-width, initial-scale=1"​ >
<title>{{ .Site.Title }}</title>
</head>
```

### themes/basico/layouts/partials/header.html

```go-html-template
<header>
<h1>{{ .Site.Title }}</h1>
</header>
<nav>
<a href=​ "/"​ >Acme</a>
<a href=​ "/viajes"​ >Viajes</a>
<a href=​ "/contacto"​ >Contacto</a>
<a href=​ "/acercade"​ >Acerca de</a>
</nav>
```

### themes/basico/layouts/partials/footer.html

```go-html-template
<footer>
  <small>Copyright {{now.Format "2022"}} Yo.</small>
</footer>
```

### themes/basico/layouts/index.html

**Para Home Page**

```go-html-template
{{ define "main" }}
{{ .Content }}
{{ end }}
```



### themes/basico/layouts/404.html

```go-html-template
{{ define "main" }}