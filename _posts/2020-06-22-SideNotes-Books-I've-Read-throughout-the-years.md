---
layout: post
title: "Books I've Read throughout the years"

categories:
  - Side Notes

tags:
  - Content
  - Side Notes
  - Books

last_modified_at: 
---


<p class="message">
  <span class="padded-dropcap">A</span> list of collective wisdom, picking up from the knowledge of many great authors.
</p>

---

<div class="dropdown" style="float:right;">
  <button class="dropbtn">In years &#x2193;</button>
  <div class="dropdown-content">
    <a href="#2022">2022</a>
    <a href="#2021">2021</a>
    <a href="#2020">2020</a>
    <a href="#2019">2019</a>
    <a href="#2018">2018</a>
    <a href="#2017">2017</a>
    <a href="#2016">2016</a>
    <a href="#2015">2015</a>
    <a href="#2011">2011</a>
  </div>
</div>

<div class="dropdown" style="float:right;">
  <button class="dropbtn">Genres &#x2193;</button>
  <div class="dropdown-content">
    <a href="#Philosophy">Philosophy</a>
    <a href="#Fiction">Fiction</a>
    <a href="#Short">Short Stories</a>
    <a href="#Business">Business</a>
    <a href="#Biography">Biography</a>
    <a href="#Women">Women Author</a>
    <div class="number">({{ entry.books | genre }})</div>
    <a href="#Men">Men Author</a>
    <a href="#Travel">Travel</a>
    <a href="#Mental Health">Mental Health</a>
  </div>
</div>

{% include books.html list=site.data.books %}


