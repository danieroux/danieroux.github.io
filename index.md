---
title: "All Conversations"
---
<ul>
{% for post in site.posts %}
<li>
      <a href="{{ post.url }}">
        {{ post.title }} on {{ post.date | date_to_long_string }}
      </a>
</li>
{% endfor %}
</ul>

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }} on {{ post.date | date_to_long_string }}
      </a>
    </h2>

    {{ post.content }}
  </article>
{% endfor %}
