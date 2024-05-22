---
layout: default
---

## Filer

<table>
  <thead>
    <tr>
      <th>Title</th>
      <th>Date</th>
      <th>URL</th>
    </tr>
  </thead>
  <tbody>
    {% for file in site.files %}
    <tr>
      <td><a href="{{ file.url }}">{{ file.title }}</a></td>
      <td>{{ file.date | date: "%Y-%m-%d" }}</td>
      <td><a href="{{ file.url }}">{{ file.url | prepend: site.github.url }}</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>
