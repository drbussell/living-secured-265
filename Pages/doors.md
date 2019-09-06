---
layout: archive
title: "Secured Doors"
permalink: "/doors/"
seotitle: "secured doors"
---

<h1 style="text-align:center;">Secured doors</h1>
<h3 class="heading-center">cam</h3>

<table class="basic-table">
	<tr>
		<th>PIC</th>
		<th>Name</th>
		<th>Price</th> 
		<th>Shop</th>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/2ZTYkLe"><img alt="Securitron BPS-12/24-1 Power Supply 12/24Vdc @ 1 Amp, Satin Chrome" class="table-image" src="/img/doors/12-24-1ps.png"/></a></td>
		<td>Securitron BPS-12/24-1 Power Supply </td>
		<td>$152.32</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/2ZTYkLe">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/34siwYm" class="table-image" src="/img/doors/ptdoorcord.png"/></a></td>
		<td>Power Transfer Door Cord</td>
		<td>$21.64</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/34siwYm">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/2PUTLki"><img alt="Lenel LNL-1320 Access Control Dual Reader Interface Module DOC-600-R" class="table-image" src="/img/doors/lnl1320.png"/></a></td>
		<td>Lenel LNL-1320 Access Control Dual Reader Interface Module DOC-600-R</td>
		<td>$499.99</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/2PUTLki">Compare Lowest Prices</a></td>
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
