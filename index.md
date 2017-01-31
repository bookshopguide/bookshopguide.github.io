---
layout: default
---

<section>
	<header class="major">
		<h2>Recommendations</h2>
	</header>
	<div class="posts">
      {% for post in site.posts %}
    <article>
        <a href="#" class="image"><img src="{{post.img}}" alt="" /></a>
        <h3>{{post.title}}</h3>
        <p>{{post.excerpt | strip_html | strip_newlines | truncate: 160}}</p>
			<ul class="actions">
				<li><a href="{{post.url | prepend: site.baseurl }}" class="button">More</a></li>
      </ul>
		</article>
        {% endfor %}
	</div>
</section>
