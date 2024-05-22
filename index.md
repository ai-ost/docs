---
layout: default
---
# AI Öst Teknik gruppen - Dokument

Välkommen till AI Öst Teknik gruppens dokumentationsrepository. Här samlar vi alla dokument och filer som vi samarbetar kring.

## Välkommen att delta i vår community!

Vi uppmuntrar nykomlingar att gå med i vår community. Det finns två sätt att göra detta:
1. Begär att bli medlem på [AI Öst GitHub](https://github.com/ai-ost).
2. Eller hitta oss på [My AI](https://my.ai.se/organizations/1816).

## Syfte

Syftet med detta repository är att tillhandahålla en central plats där alla medlemmar i AI Öst Teknik gruppen kan skapa, redigera och samarbeta kring dokument. Detta inkluderar tekniska specifikationer, mötesanteckningar, projektplaner och andra viktiga filer.

## Filer

<table class="padded-table aligned-table">
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
