---
defaults:
# _pages
- scope:
path: ""
type: pages
values:
layout: home
author_profile: true	
permalink: /
image_path: assets/images/MV2021_postal_web.jpg
---
Hello index

<div class="newsFlash">
<ul>
{% for member in site.data.news %}
  <li>
	 <img src="{{ member.imgage  }}" />
     <h4> {{ member.title }} </h4>
     <p> {{ member.text }} </p>
  </li>
{% endfor %}
</ul>
</div>

