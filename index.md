---
# the title that will appear in the HTML head tag
layout: wrapper
title: index home page
food: pizza
---

## Learn Guitar Home page

<div class="bacon" markdown="1">
  
It **works!**
  
</div>

<h1>{{ page.food }}</h1>

## Images

![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

{% for staff_member in sitemy_collections.staff_members %}
  <h1>{{ staff_member.name }} - {{ staff_member.position }}</h1>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}

{% for book in site.my_collections.books %}
  <h2>{{ book.name }} - {{ book.position }}</h2>
  <p>{{ book.content | markdownify }}</p>
{% endfor %}