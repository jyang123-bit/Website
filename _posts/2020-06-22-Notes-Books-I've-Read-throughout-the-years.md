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
<h2>Books I've Read</h2>

<p class="message">
  A list of collective wisdom, picking up from the knowledge of many great authors.
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

  <div class="posts">
  
    {% assign books = site.books | sort: "date" | reverse %}

    {% for book in books %}
  	<div class="post-teaser book-teaser">
  		<div>
			<a href="{{ book.url | prepend: site.baseurl }}">
  			    <img class="book-cover book-cover-teaser" src="/wp-content/covers/{{ book.cover }}">
                    </a>
  		</div>
		<div class="book_info">
		  	<div class="book_meta">
			  	<h3><em><a href="{{ book.url | prepend: site.baseurl }}">{{ book.title }}</a></em></h3>
			  	<p>Author: {{ book.author }}</p>
				<p>Read: {{ book.date | date_to_string }}</p> 
			  	<a class="button" href="{{ book.url | prepend: site.baseurl }}">Read full notes</a>
		  	</div>
	  	</div>

  	</div>
  {% endfor %}


 </div>


