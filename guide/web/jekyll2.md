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

[Montrer les dernières publications d'un blog](https://stackoverflow.com/questions/17890493/how-can-i-show-just-the-most-recent-post-on-my-home-page-with-jekyll)

[Doc : Posts, catérogies, tags, extraits, brouillons](https://jekyllrb.com/docs/posts/)

[Site multilingue avec Jekyll](https://www.sylvaindurand.org/making-jekyll-multilingual/)

`jekyll serve --drafts` pour voir les brouillons (_drafts) comme si ils étaient dans les publications (_posts)
