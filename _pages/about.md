---
defaults:
# _pages
- scope:
path: ""
type: pages
values:
layout: single
author_profile: true	
permalink: /about/
---
This site is dedicated to sharing information about what I do as a musician, composer and researcher. The site is definitely an infinite work-in-progress and perhaps more of an archive than a promotion. I do however use this site, among other things, as a virtual stage posting new recordings and pieces every now and then.

{% assign bio = site.data.web_bio | sort: 'lang' %}
{% for member in bio %}
  <li>
     <h4> {{ member.title }} </h4>
	 <p> {{ member.date }} </p>
     <p> {{ member.text }} </p>
  </li>
{% endfor %}
