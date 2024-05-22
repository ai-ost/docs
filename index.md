---
layout: default
---

## Filer

<table>
  <thead>
    <tr>
      <th>Title</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    {% for file in site.files %}
    <tr>
      <td><a href="{{ file.url  | prepend: site.baseurl }}">{{ file.title }}</a></td>
      <td>{{ file.date | date: "%Y-%m-%d" }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
