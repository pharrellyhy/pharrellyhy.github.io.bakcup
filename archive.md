---
layout: page
title: Archive
---
<hr>
<div class="posts">
    {% for post in site.posts %}    
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p><small>{{ post.date | date: "%b %d %Y" }} {{ post.category }} <a href="http://erjjones.github.com{{ post.url }}#disqus_thread"></a></small></p>
    {% endfor %}
</div>