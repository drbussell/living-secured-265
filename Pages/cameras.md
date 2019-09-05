---
layout: archive
title: "security cameras"
permalink: "/cameras/"
seotitle: "security cameras"
---

<h1 style="text-align:center;">Security Cameras</h1>
<h3 class="heading-center">cam</h3>

<table class="basic-table">
	<tr>
		<th>PIC</th>
		<th>Name</th>
		<th>Price</th> 
		<th>Shop</th>
	</tr>
	<tr>
		<td><a target="_blank" href=""><img alt="cam" class="table-image" src="/img/bongs/.png"/></a></td>
		<td>cam</td>
		<td>$</td>
		<td><a class="big-button" target="_blank" href="">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="" class="table-image" src="/img/bongs/.png"/></a></td>
		<td>cam</td>
		<td>$</td>
		<td><a class="big-button" target="_blank" href="">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="l"><img alt="cam" class="table-image" src="/img//.png"/></a></td>
		<td>cam</td>
		<td>$</td>
		<td><a class="big-button" target="_blank" href="">Compare Lowest Prices</a></td>
	</tr>
</table>
 <nav>

<ul class="taxonomy__index">
  {% assign postsInYear = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}
  {% for year in postsInYear %}
    <li>
      <a href="#{{ year.name }}">
        <strong>{{ year.name }}</strong> <span class="taxonomy__count">{{ year.items | size }}</span>
      </a>
    </li>
  {% endfor %}
</ul>

{% assign postsByYear = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}
{% for year in postsByYear %}
  <section id="{{ year.name }}" class="taxonomy__section">
    <h2 class="archive__subtitle">{{ year.name }}</h2>
    <div class="entries-{{ page.entries_layout | default: 'list' }}">
      {% for post in year.items %}
        {% include archive-single.html type=page.entries_layout %}
      {% endfor %}
    </div>
    <a href="#page-title" class="back-to-top">{{ site.data.ui-text[site.locale].back_to_top | default: 'Back to Top' }} &uarr;</a>
  </section>
{% endfor %}
