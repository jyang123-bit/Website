---
layout: post
title: "Books I've Read throughout the years"

categories:
  - Notes

tags:
  - Content
  - Notes
  - Books

last_modified_at: 
---

<p class="message">
  <span class="padded-dropcap">A</span> list of collective wisdom, picking up from the knowledge of many great authors.
</p>

<div class="dropdown" style="float:right;">
  <button class="dropbtn">In years</button>
  <div class="dropdown-content">
    <a href="#2020">2020</a>
    <a href="#2019">2019</a>
    <a href="#2018">2018</a>
    <a href="#2017">2017</a>
    <a href="#2016">2016</a>
    <a href="#2015">2015</a>
    <a href="#2014">2014</a>
    <a href="#2013">2013</a>
    <a href="#2012">2012</a>
    <a href="#2011">2011</a>
    <a href="#2010">2010</a>
  </div>
</div>

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
          <span class="author">by {{ book.author }}</span
          >{% if book.star %}<span class="star">★</span>{% endif %}
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
  {% endfor %}
</div>  

