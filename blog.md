---
layout: french
title: Blogs
---
# Billets
Les billets qui présentent la vie de la maison du jardinier
{% for post in site.posts %}
{{ post.date | date_to_string }} [{{ post.title }}]({{ post.url }})
{% endfor %}


# billets des travaux
{% for post in site.categories.travaux %}
{{ post.date | date_to_string }} [{{ post.title }}]({{ post.url }})
{% endfor %}
