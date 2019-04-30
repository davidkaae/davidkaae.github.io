<!-- ## Pages -->

<!-- <ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul> -->

<!-- <h2>Categories</h2>
{% for category in site.categories %}
<div style="display:inline-block; margin-right: 20px;">
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
  </div>
{% endfor %} -->

{{ content }}