---
name: Francophonie
summary: Posts related to francophonie
author: Hilquias Ferreira
image: ../assets/img/categ/french-language.png
---

<h3>Posts by category</h3>

{% for post in site.categories.francophonie %}
<div class="col-md-10 blogShort">
    <h1>{{post.title | escape}}</h1>
    <!--
    <img src="{{ post.thumbnail }}" alt="post img"
    class="pull-left img-responsive thumb margin10 img-thumbnail">
    -->
    {%- for tag in post.categories -%}
    <a href="#" class="badge badge-primary"> {{ tag }} </a>
    {%- endfor -%}

    <article>
        <p>
            {{ post.summary }}
        </p>
    </article>
    <a class="btn btn-outline-primary" href="{{ post.url }}">READ MORE</a>
</div>
{% endfor %}