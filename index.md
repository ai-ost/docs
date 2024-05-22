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
      <td><a href="{{ file.url  | prepend: site.baseurl }}">{{ file.title }}</a></td>
      <td>{{ file.date | date: "%Y-%m-%d" }}</td>
      <td><a href="{{ file.url | prepend: site.baseurl }}">{{ file.url | prepend: site.baseurl }}</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>
