---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<img src="{{site.baseurl}}/assets/images/phi.png">
<h3>This is a philosophy blog without too many thrills. What matters is the ideas.</h3>

{%- assign latest_post = site.posts[0] -%}
<h2>Latest Post: <a href="{{ latest_post.url }}">{{ latest_post.title }}</a></h2>

<!-- {% for post in site.posts limit:1 %}
<li>
    <a href="{{ post.url }}">
    <h3>{{ post.title }}</h3>
    </a>
</li>
{% endfor %}
<h1>Recent Posts</h1>
{% for post in site.posts offset:1 limit:2 %}
<li>
    <a href="{{ post.url }}">
    <h3>{{ post.title }}</h3>
    </a>
</li>
{% endfor %} -->