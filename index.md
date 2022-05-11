---
layout: default
---

This is the website of Deryk Makgill. I write about psychology, statistics, and technology. I am best known for work on the darknet markets & Bitcoin⁠, blinded self-experiments⁠, dual n-back & spaced repetition⁠, and anime neural networks⁠.

[Click here](/about) for personal and contact information.

[Click here](/rss) for RSS feed or [here](/) for my newsletter.

[Click here](/random) for something random.

---

{% assign tweets = site.tweets | sort: 'date' | reverse %}
{% for tweets in tweets %}
 
<div class="tweet" style="margin-bottom:1em;"><a href="{{ tweets.url | prepend: site.baseurl }}">
{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
<span class="dt-published" style="display:inline;"datetime="{{ tweets.date | date_to_xmlschema }}" itemprop="datePublished">
{{ tweets.date | date: date_to_rfc822 }}
 </span></a> {{ tweets.content | truncate: 445 }}</div>
 

{% endfor %}  

---

