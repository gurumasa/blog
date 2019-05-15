---
layout: archive
author_profile: true

title: Aiheet

excerpt: "Blogikirjoitukset aiheittain."
header:
  overlay_image: /assets/images/header4.jpg
  overlay_filter: 0.2 # same as adding an opacity of 0.5 to a black background
  caption: "**Waterlow Park, Highgate**"
---

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
