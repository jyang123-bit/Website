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
    <a href="#2020">2020</a>
    <a href="#2019">2019</a>
    <a href="#2018">2018</a>
    <a href="#2017">2017</a>
    <a href="#2016">2016</a>
    <a href="#2015">2015</a>
    <a href="#2011">2011</a>
  </div>
</div>

{% endcase %}
<link rel="stylesheet" href="{{ site.baseurl }}/_sass/jingyuh.scss">

<div class="booklist">
  <div class="last-update">Last updated {{ site.data.books.lastupdate }}</div>
  {% for entry in site.data.books.list %}
  <div class="year-container">
    <div class="year">
      <h4>{{ entry.year }}</h4>
      <div class="number">{{ entry.books | size }} books</div>
    </div>
    <div class="books">
      <ul class="books{{ entry.year }}">
        {% for book in entry.books %}
        <li>
          <a href="{{ book.link }}" alt="_blank" rel="nofollow noopener">{{
            book.title
          }}</a>
          <p>Author: {{ book.author }}</p>
          <p>Published: {{ book.published }}</p>
          <p>Pages: {{ book.pages }}</p>
          <p>Genre: {{ book.genre }}</p>
          {% if book.star %}<span class="star">★</span>{% endif %}
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
  {% endfor %}
</div>  

