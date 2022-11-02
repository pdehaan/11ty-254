---
title: Content Title
permalink: /
eleventyExcludeFromCollections: true
---

# {{ title }}

{% for p in collections.chapters %}
<section data-file-slug="{{ p.fileSlug }}" data-order="{{ p.data.order }}">
  {{ p.templateContent }}
</section>
{% endfor %}
