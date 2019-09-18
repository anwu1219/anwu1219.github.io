<div>
  <ul>
    {% for post in site.categories.science %}
        <li>
        {{ post.ref-authors }},
        {{ post.ref-title }}.
        <em>{{ post.ref-journal}}.</em>
        [<a href="{{ site.url }}/{{ post.ref-file }}">pdf</a>]
        {% if post.ref-url %}
        [<a href="{{ post.ref-url }}">project</a>]
        {% endif %}
        </li>
    {% endfor %}
  <ul>