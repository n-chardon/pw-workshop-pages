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
{% for page in site.html_pages %}
<li>
    <a href="{{ page.url }}">{{ page.title }}</a>
</li>
{% endfor %}
</ul>

<ul>
{% for post in site.posts %}
<li>
    <a href="{{ post.url }}">{{ post.title }}</a>
</li>
{% endfor %}
</ul>