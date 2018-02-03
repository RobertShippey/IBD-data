---
layout: layout
title: IBD Open Data
description: " "
---

Here is a collection of data sets relating to IBD, Crohn's Disease, and Ulcerative Colitis. If you have any suggestions, tweet me [@robertshippey](https://twitter.com/robertshippey) or [open an Issue on Github](https://github.com/RobertShippey/IBD-data). 

Openness and transparency are important, open data sets are key to this. 

{% for post in site.posts %}

{% cycle '<div class="row">', ' ', ' ' %}

	<div class="col-sm-6 col-md-4">
		<div class="panel panel-default">
			<div class="panel-heading">
				<h3 class="panel-title">{{ post.title }}
					{% if post.datasize %}<span class="badge">{{ post.datasize }}</span>{% endif %}
				</h3>
			</div>
			<div class="panel-body">
				{{ post.content }}
			</div>
			<div class="panel-footer">
				<a href="{{ post.link }}" target="_blank" rel="noopener noreferrer">
					{% if post.glyphicon %}<span class="glyphicon glyphicon-{{ post.glyphicon }}" aria-hidden="true"></span> {% endif %}
				Visit</a>
			</div>
		</div>
	</div>

{% cycle ' ', ' ', '</div>' %}

{% endfor %}