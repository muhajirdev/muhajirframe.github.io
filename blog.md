---
layout: blog
title: Blog
permalink: /blog/
gambar: /img/koran.png
skills: Thoughts, stories and ideas.
---
<section>
	<div class="container">
		<div class="row">
			<div class=" col-xs-10 col-xs-offset-1 col-lg-8 col-lg-offset-2  post-list">
				{% for post in site.posts %}
							<a class="post-link" href="{{ post.url | prepend: site.baseurl }}"><h2>{{ post.title }}</h2></a>
								<p>
									{{post.description}}
								</p>
								<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
						<hr>
				{% endfor %}

			</div>
		</div>
	</div>
</section>
