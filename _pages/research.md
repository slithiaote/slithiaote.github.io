---
title: Thèmes de recherche
layout: single
permalink: /research/
classes: wide
---

- Analyse d'images et traitement du signal
- Imageries biomédicales
- Statistique
- Analyse de données et apprentissage

{% comment %}
# Encadrement
- co-direction de trois thèses de doctorat : Dai Viet Tran, [Duc Nghia Tran](/research/rpe), [Safaa Al Ali](/research/safaa)
- co-encadrement de quatre stages de M2
{% endcomment %}

# Projets

{% case site.tag_archive.type %}
  {% when "liquid" %}
    {% assign path_type = "#" %}
  {% when "jekyll-archives" %}
    {% assign path_type = nil %}
{% endcase %}

<div class="feature__wrapper">
{% assign entries = site["research"] | sort: "project_end" | reverse %}
{%- for post in entries -%}
  {%- unless post.hidden -%}
    <div class="feature__item--left">
      <div class="archive__item">
        {% if post.header.teaser %}
          <div class="archive__item-teaser">
            <img src="{{ post.header.teaser | relative_url }}" alt="">
          </div>
        {% endif %}

        <div class="archive__item-body">
          {% if post.title %}
            <h2 class="archive__item-title"><a href="{{ post.url | relative_url }}" rel="permalink">{{ post.title }}</a></h2>
          {% endif %}

          {% if post.excerpt %}
            <div class="archive__item-excerpt">
              {{ post.excerpt | markdownify }}
          {% if site.tag_archive.type and post.tags[0] %}
					  {% assign tags_sorted = post.tags | sort_natural %}
            <p class="page__taxonomy">
            <span itemprop="keywords">
            {% for tag_word in tags_sorted %}
            <a href="{{ tag_word | slugify | prepend: path_type | prepend: site.tag_archive.path | relative_url }}" class="page__taxonomy-item p-category" rel="tag">{{ tag_word }}</a>{% unless forloop.last %}<span class="sep">, </span>{% endunless %}
            {% endfor %}
						{{post.project_date}}
            </span>
            </p>
          {% endif %}
            </div>
          {% endif %}

        </div>
      </div>
    </div>

    
  {%- endunless -%}
{%- endfor -%}
</div>
