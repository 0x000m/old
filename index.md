---
layout: default
---

This is the website of Deryk Makgill. I write about psychology, statistics, and technology. I am best known for work on the darknet markets & Bitcoin⁠, blinded self-experiments⁠, dual n-back & spaced repetition⁠, and anime neural networks⁠.

<p class="tweet"><a href="/">BUY</a> YOUR SQUARE OF DIGITAL REAL ESTATE ON THIS SITE AND HAVE YOUR NAME, MESSAGE, AND ART HOSTED FOR LIFE. </p>

---

[Click here](/about) for personal and contact information.

[Click here](/rss) for RSS feed or [here](/) for my newsletter.

[Click here](/random) for something random.

<hr>

{% assign tweets = site.tweets | sort: 'date' | reverse %}
{% for tweets in tweets %}


 
 
<div class="tweet" style="margin-bottom:1em;">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
       {{ tweets.date | date_to_long_string }}: {{ tweets.content | truncate: 445 }}</div>
 

{% endfor %}  
<hr>

{% assign changelog = site.changelog | sort: 'date' | reverse %}
{% for changelog in changelog %}


 
 
<div class="tweet" style="margin-bottom:1em;">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      {{ changelog.date | date_to_long_string }}: {{ changelog.content | truncate: 445 }}</div>
 

{% endfor %}  

---

Last modified: 11 May 2022<br>
[Deryk Makgll](/) 1930 Airlane Drive, Nashville, TN 37210
