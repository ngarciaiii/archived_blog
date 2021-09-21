---
layout: default
title: About
---

<h3></h3>
![profpic](/public/img/profpic.jpeg){: .colright, .prof_pic }

<about-short> 
<h1>Nicolas Garcia III</h1>
<h1><a href="https://ngarciaiii.github.io/blog#">I blog what I learn</a></h1><h3></h3>
<short-headline>Researchings, programmings, and things I apply in my life. <br><br/>
</short-headline>


<div class="abt-personal-info">
  {% if site.author.contact %}
  {% assign len = site.author.contact | size %}
  {% assign current_index = 0 %}
  <div class="abt-personal-info-section">
    <div class="abt-background">
      {% for contact in site.author.contact %}
      {% assign iconname = contact[0] %}
      {% if contact[0] == 'email' %}
      {% assign iconname = 'envelope' %}
      {% endif %}
      <a href="{{ contact[1] }}">
        <i class="fa fa-{{ iconname }}" aria-hidden="true"></i>
      </a>
      {% assign current_index = current_index | plus: 1 %}
      {% if current_index != len %}  {% endif %}
      {% endfor %}
      </div>
  </div>
</div>
{% endif %}

<style >
  
  short-headline {
    font-size: 1.2rem;
  }

  h1 a:hover {
      text-decoration: none;
      /* font-size: 1.97rem; */
      /* font-weight: 510; */
      color: #70c137;
  }

  about-short {
    float:right;
    width: 50%;
    margin-top: -1.43rem;
  }

</style>