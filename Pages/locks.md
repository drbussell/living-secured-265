---
layout: archive
title: "Door Locks"
permalink: "/locks/"
seotitle: "best locks"
---

<h3 class="heading-center">Electric stikes</h3>

<table class="basic-table">
	<tr>
		<th>PIC</th>
		<th>Name</th>
		<th>Price</th> 
		<th>Shop</th>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/2ZQFtkr"><img alt="HES 5000 Series Stainless Steel Compact High Performance Electric Strike Body, Satin Stainless Steel Finish" class="table-image" src="/img/locks/5000strike.png"/></a></td>
		<td>HES 1500 Series electric strike</td>
		<td>$100</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/2ZQFtkr">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/2MU6525"><img alt="HES 5200 Series Stainless Steel" class="table-image" src="/img/locks/5200strike.png"/></a></td>
		<td>HES 5200 Series Stainless Steel</td>
		<td>$88</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/2MU6525">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/2Uug8f6"><img alt="HES 4500 Series Stainless Steel Low Profile Heavy Duty and Fire Rated Electric Strike Body, Satin Stainless Steel Finish" class="table-image" src="/img/locks/4500strike.png"/></a></td>
		<td>HES 4500 Series Stainless Steel</td>
		<td>$335.42</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/2Uug8f6">Compare Lowest Prices</a></td>
	</tr>
</table>

<h3 class="heading-center">Magnalocks</h3>

<table class="basic-table">
	<tr>
		<th>PIC</th>
		<th>Name</th>
		<th>Price</th> 
		<th>Shop</th>
	</tr>
	<tr>
		<td><a target="_blank" href="https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338330075&mpre=https%3A%2F%2Fwww.ebay.com%2Fitm%2FSecuritron-IMXDA-Integrated-Motion-Exit-Delay-Model-62-Holding-1200-lbs%2F143208888272%3Fepid%3D1019233610%26hash%3Ditem2157ea37d0%3Ag%3AspIAAOSwmMNcRLuR%3Asc%3AFedExHomeDelivery!21702!US!-1"><img alt="Securitron IMXDA Integrated Motion Exit Delay Model 62 Holding 1200 lbs" class="table-image" src="/img/locks/imxdamag.png"/></a></td>
		<td>Securitron IMXDA Integrated Motion Exit Delay Model 62</td>
		<td>$399.95</td>
		<td><a class="big-button" target="_blank" href="https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338330075&mpre=https%3A%2F%2Fwww.ebay.com%2Fitm%2FSecuritron-IMXDA-Integrated-Motion-Exit-Delay-Model-62-Holding-1200-lbs%2F143208888272%3Fepid%3D1019233610%26hash%3Ditem2157ea37d0%3Ag%3AspIAAOSwmMNcRLuR%3Asc%3AFedExHomeDelivery!21702!US!-1">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338330075&mpre=https%3A%2F%2Fwww.ebay.com%2Fsch%2Fi.html%3F_from%3DR40%26_trksid%3Dm570.l1313%26_nkw%3DSecuritron%2BM32%2BMagnalock%26_sacat%3D0"><img alt="Securitron M32 Magnalock" class="table-image" src="/img/locks/m32mag.png"/></a></td>
		<td>Securitron M32 Magnalock</td>
		<td>$200</td>
		<td><a class="big-button" target="_blank" href="https://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_id=114&ipn=icep&toolid=20004&campid=5338330075&mpre=https%3A%2F%2Fwww.ebay.com%2Fsch%2Fi.html%3F_from%3DR40%26_trksid%3Dm570.l1313%26_nkw%3DSecuritron%2BM32%2BMagnalock%26_sacat%3D0">Compare Lowest Prices</a></td>
	</tr>
	<tr>
		<td><a target="_blank" href="https://amzn.to/2Uug8f6"><img alt="HES 4500 Series Stainless Steel Low Profile Heavy Duty and Fire Rated Electric Strike Body, Satin Stainless Steel Finish" class="table-image" src="/img/locks/4500strike.png"/></a></td>
		<td>HES 4500 Series Stainless Steel</td>
		<td>$335.42</td>
		<td><a class="big-button" target="_blank" href="https://amzn.to/2Uug8f6">Compare Lowest Prices</a></td>
	</tr>
</table>
 

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
