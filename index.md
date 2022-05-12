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
       {{ tweets.date | date_to_long_string }}: {{ tweets.content | truncate: 445 }}</div>
 

{% endfor %}  

<hr>

<div class="container">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/1610_Cecco_del_Caravaggio_Christ_expulses_money_changers_anagoria.JPG/1599px-1610_Cecco_del_Caravaggio_Christ_expulses_money_changers_anagoria.JPG?20120904164840" alt="Snow" style="width:100%;">
  <div class="centered">
Woe unto you, scribes and Pharisees, hypocrites! because ye build the tombs of the prophets, and garnish the sepulchres of the righteous. And say, If we had been in the days of our fathers, we would not have been partakers with them in the blood of the prophets.. Wherefore ye be witnesses unto yourselves, that ye are the children of them which killed the prophets. Fill ye up then the measure of your fathers. Ye serpents, ye generation of vipers, how can ye escape the damnation of hell?</div>
</div>

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
