---
layout: splash
title: "Chenyu Lu"
header:
  image: "profile.png"
excerpt: "Computer Science & Mathematics student at HKUST working on cryptography, blockchain protocols, and AI systems."
---

<div class="wrapper">

<p>{{ site.author.name }} — {{ site.author.bio }}</p>

**🔥 News**

<ul>
{% raw %}{% for post in site.posts limit:5 %}{% endraw %}
  <li>{{ "{{ post.date | date: \"%Y.%m\" }}" }} — <a href="{{ "{{ post.url }}" }}">{{ "{{ post.title }}" }}</a></li>
{% raw %}{% endfor %}{% endraw %}
</ul>

**🛠️ Projects**

<ul>
{% raw %}{% for proj in site.portfolio limit:5 %}{% endraw %}
  <li><a href="{{ "{{ proj.url }}" }}">{{ "{{ proj.title }}" }}</a></li>
{% raw %}{% endfor %}{% endraw %}
</ul>

**📚 Publications**

<ul>
{% raw %}{% for pub in site.publications limit:5 %}{% endraw %}
  <li>{{ "{{ pub.date | date: \"%Y\" }}" }} — <a href="{{ "{{ pub.url }}" }}">{{ "{{ pub.title }}" }}</a></li>
{% raw %}{% endfor %}{% endraw %}

<p><a href="/files/CV.pdf">Download CV</a></p>

</div>
