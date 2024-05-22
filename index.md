---
layout: default
---

## Filer

| Titel | Datum | URL |
|-------|------|-----|
{% for file in site.files %}
| [{{ file.title }}]({{ file.url | prepend: site.baseurl }}) | {{ file.date | date: "%Y-%m-%d" }} | [{{ file.url | prepend: site.baseurl }}]({{ file.url | prepend: site.baseurl }}) |
{% endfor %}
