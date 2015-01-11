---
layout: pageminimal
title: Archives Index
permalink: /archives/index.html
title: Time Machine
description: "An archive of post "

---
<h2>Time Machine</h2>
<ul class="post-list">
                {% for post in site.posts %}
                   <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time></a></li>
                {% endfor %}
              </ul>
              
             