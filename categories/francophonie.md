---
layout: categories
name: Dynamics 365 FO
---


{% for post in site.categories.francophonie %}
<div class="col-md-10 blogShort">
    <h1>{{post.title | escape}}</h1>
    
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