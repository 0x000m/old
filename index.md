---
layout: default
---

This is the website of Deryk Makgill. I write about [Bitcoin](/), [old books](/), and [technology](/). I am best known for work on the [darknet markets](/) & [Bitcoin⁠](/), [blinded self-experiments](/)⁠, [dual n-back & spaced repetition⁠](/), and [anime neural networks](/)⁠.

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
  <img src="https://i.imgur.com/1UnNP6B.png" alt="Snow" style="width:100%;">
  <div class="top-left" style="font-size:6em;font-weight:bold; font-family:serif;">
Essays</div>
</div>

- [The Family of the Vourdalak](/) by Alexei Tolstoy (1884) -- [html](/) (138K) -- [pdf](/) (138K)

---

<div class="container">
  <img src="https://i.imgur.com/MeUkmXV.png" alt="Snow" style="width:100%;">
  <div class="top-right" style="font-size:6em;font-weight:bold; font-family:serif;">
Reviews</div>
</div>


- [The Family of the Vourdalak](/) by Alexei Tolstoy (1884) -- [html](/) (138K) -- [pdf](/) (138K)

---

<div class="container">
  <img src="https://live.staticflickr.com/3784/13946155583_e385bfc147_b.jpg" alt="Snow" style="width:100%;">
  <div class="bottom-right" style="font-size:6em;font-weight:bold; font-family:serif;">
Interviews</div>
</div>


- [The Family of the Vourdalak](/) by Alexei Tolstoy (1884) -- [html](/) (138K) -- [pdf](/) (138K)

---

<div class="container">
  <img src="https://artuk.org/download/the-scribe-68808" alt="Snow" style="width:100%;">
  <div class="bottom-left" style="font-size:6em;font-weight:bold; font-family:serif;">
Translations</div>
</div>

- [The Family of the Vourdalak](/) by Alexei Tolstoy (1884) -- [html](/) (138K) -- [pdf](/) (138K)

---

#### Changelog

{% assign changelog = site.changelog | sort: 'date' | reverse %}
{% for changelog in changelog %}


 
 
<div class="tweet" style="margin-bottom:1em;">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      {{ changelog.date | date_to_long_string }}: {{ changelog.content | truncate: 445 }}</div>
 

{% endfor %}  

---

Last modified: 11 May 2022<br>
[Deryk Makgll](/) 1930 Airlane Drive, Nashville, TN 37210
