---
title: Accueil du site 
description: Exemple d'usage de Jekyll sur Github Pages
---
# Paris Web

## Atelier du 6 octobre

Texte de la page

{{site.title}}

{{site.description}}

<h1>{{page.title}}</h1>
Menu : 
<ul>
{% for page in site.pages %}
<li>
    <a href="{{ page.url }}">{{ page.title }}</a>
</li>
{% endfor %}
</ul>