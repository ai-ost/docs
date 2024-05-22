---
layout: default
---

## Filer

<table>
  <thead>
    <tr>
      <th style="text-align: left">Title</th>
      <th style="text-align: right">Date</th>
    </tr>
  </thead>
  <tbody>
    {% for file in site.files %}
    <tr>
      <td style="text-align: left"><a href="{{ file.url  | prepend: site.baseurl }}">{{ file.title }}</a></td>
      <td style="text-align: right">{{ file.date | date: "%Y-%m-%d" }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
