---
layout: null
---
# Collections Dir Traversal

## All collections:
{% for collection in site.collections %}
- {{ collection.label }}: {{ collection.docs | size }} docs
  {% for doc in collection.docs %}
  - {{ doc.path }}
  {% endfor %}
{% endfor %}
