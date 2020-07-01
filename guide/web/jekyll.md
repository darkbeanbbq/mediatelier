# Jekyll


[Using an image caption in Markdown Jekyll :](https://stackoverflow.com/questions/19331362/using-an-image-caption-in-markdown-jekyll/30366422#30366422)

Créer un `image.html` dans `_includes` tel que :

```
<figure class="image">
  <img src="{{ include.url }}" alt="{{ include.description }}">
  <figcaption>{{ include.description }}</figcaption>
</figure>
```

```
{% include image.html url="/images/my-cat.jpg" description="My cat, Robert Downey Jr." %}
```
---
