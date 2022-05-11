---
layout: default
---

This is the website of Deryk Makgill. I write about psychology, statistics, and technology. I am best known for work on the darknet markets & Bitcoin⁠, blinded self-experiments⁠, dual n-back & spaced repetition⁠, and anime neural networks⁠.

---

[Click here](/about) for personal and contact information.

[Click here](/rss) for RSS feed or [here](/) for my newsletter.

[Click here](/random) for something random.

<hr>

{% assign tweets = site.tweets | sort: 'date' | reverse %}
{% for tweets in tweets %}


 
 
<div class="tweet" style="margin-bottom:1em;">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ tweets.date | date: date_to_rfc822 }}: {{ tweets.content | truncate: 445 }}</div>
 

{% endfor %}  
<hr>

{% assign changelog = site.changelog | sort: 'date' | reverse %}
{% for changlog in changelog %}


 
 
<div class="changelog" style="margin-bottom:1em;">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ changelog.date | date: date_to_rfc822 }}: {{ changelog.content | truncate: 445 }}</div>
 

{% endfor %}  

All written materials on this Web site are my own, and all are released under the Do What the Fuck You Want to Public License Version 2.

