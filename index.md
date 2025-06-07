---
layout: default
title: Mi primer Sitio Jekyll
header_image: destacada.jpg
---

# Mi primer Sitio Jekyll

## Último Post

{% assign primer_post = site.posts | where: "path", "_posts/2025-05-24-mi-primer-post.md" | first %}

{% if primer_post %}
### {{ primer_post.title }}
{{ primer_post.content }}
{% else %}
<p>No se encontró el post. Verifica que el archivo exista en _posts/</p>
{% endif %}