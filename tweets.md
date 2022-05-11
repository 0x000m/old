---
layout: default
---

<h1>Tweets, Twetches, etc...</p></h1>

{% assign tweets = site.tweets | sort: 'date' | reverse %}
{% for tweets in tweets %}


 
 
<div class="tweet" style="margin-bottom:1em;">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ tweets.date | date: date_to_rfc822 }} {{ tweets.content | truncate: 445 }}</div>
 

{% endfor %}  
