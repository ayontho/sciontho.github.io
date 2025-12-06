---
layout: page
title: Sci-on
permalink: /
---

<div class="poem-block" markdown="1">

  Let's try and think like Tinbergen:

***One**, "It's thus. What makes it so?"*  
***Two**, "Huh. But why should it be so?"*  
***Three**, "How has it come to be,*  
*What ingredients make the recipe?"*  
***Finally**, it must be solved*  
*How on earth has this evolved?*  

</div>

---

Welcome, welcome!

Tinbergen reckons that to understand behaviour, one must ask questions of four kinds - questions on "Causation", "Function", "Development" and "Evolution". And this shall serve as the foundation for the kinds of papers we’ll geek out on. So, we'll look at:

- **Causation** – What immediate processes cause the behaviour?  
- **Development** – How does the behaviour emerge?  
- **Function** – Why does it exist? What does it do for the animal?  
- **Evolution** – How did it arise over time?

We’ll interpret these terms freely (you’ll see!). Overall, though, these four lenses guide how I read papers and think about science.

Use the navigation bar above to explore.

---

# Featured

<div class="featured-grid">

  {% assign powwow_posts = site.posts | where_exp:"p","p.categories contains 'pow-wow'" %}
  {% assign powwow_post = powwow_posts | first %}
  {% if powwow_post %}
  <a href="{{ powwow_post.url | relative_url }}" class="featured-card">
    <img src="{{ powwow_post.thumbnail | default: '/assets/img/sci-art/Sciontho.png' }}" alt="{{ powwow_post.title }}">
    <div class="featured-title">Pow-wow: {{ powwow_post.title }}</div>
  </a>
  {% endif %}

  {% assign sciart_posts = site.posts | where_exp:"p","p.categories contains 'sci-art'" %}
  {% assign sciart_post = sciart_posts | first %}
  {% if sciart_post %}
  <a href="{{ sciart_post.url | relative_url }}" class="featured-card">
    <img src="{{ sciart_post.thumbnail | default: '/assets/img/sci-art/MirrorMirror.png' }}" alt="{{ sciart_post.title }}">
    <div class="featured-title">Sci-art: {{ sciart_post.title }}</div>
  </a>
  {% endif %}

  {% assign drawn_posts = site.posts | where_exp:"p","p.categories contains 'drawn-to-science'" %}
  {% assign drawn_post = drawn_posts | first %}
  {% if drawn_post %}
  <a href="{{ drawn_post.url | relative_url }}" class="featured-card">
    <img src="{{ drawn_post.thumbnail | default: '/assets/img/sci-art/DBJC.png' }}" alt="{{ drawn_post.title }}">
    <div class="featured-title">Drawn to science: {{ drawn_post.title }}</div>
  </a>
  {% endif %}

  {% assign archive_posts = site.posts | where_exp:"p","p.categories contains 'archive'" %}
  {% assign archive_post = archive_posts | first %}
  {% if archive_post %}
  <a href="{{ archive_post.url | relative_url }}" class="featured-card">
    <img src="{{ archive_post.thumbnail | default: '/assets/img/sci-art/MyPhD.png' }}" alt="{{ archive_post.title }}">
    <div class="featured-title">From the archive: {{ archive_post.title }}</div>
  </a>
  {% endif %}

</div>
