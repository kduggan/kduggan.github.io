---
layout: page
title: Latest Post
---
{% include JB/setup %}
<div class="blog-index">
{% assign post = site.posts.first %}
{% assign content = post.content %}
{% include post_detail.html %}

</div>

 <hr>
 <ul class="pagination">
    {% if page.previous %}
 <li class="prev"><a href="{{ BASE_PATH }}{{ page.previous.url }}" title="{{ page.previous.title }}">&laquo; Previous</a></li>
    {% else %}
 <li class="prev disabled"><a>&larr; Previous</a></li>
    {% endif %}
  <li><a href="{{ BASE_PATH }}{{ site.JB.archive_path }}">Archive</a></li>
    {% if page.next %}
  <li class="next"><a href="{{ BASE_PATH }}{{ page.next.url }}" title="{{ page.next.title }}">Next &raquo;</a></li>
    {% else %}
  <li class="next disabled"><a>Next &rarr;</a>
   {% endif %}
 </ul>



