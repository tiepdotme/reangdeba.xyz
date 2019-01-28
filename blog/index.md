---
layout: blog
title: blog
---
<ul class="list">
  {% for post in site.posts %}
  <div class="mv2">
  <li>
    <a href="{{ site.url }}{{ post.url }}" class="db pv1 link blue hover-mid-gray">
      <time class="fr silver ttn">{{ post.date | date_to_string }} </time>
      {{ post.title }}
    </a>
  </li>
  </div>
  {% endfor %}
</ul>
