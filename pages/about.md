---
layout: page
title: About
description: A Android developer, expert in Android who lives in Beijing.
keywords: Amphiaraus,Android
comments: true
menu: 关于
permalink: /about/
---

A Android developer, expert in Android who lives in Beijing.

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
