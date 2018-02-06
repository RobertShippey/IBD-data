---
layout: layout
title: IBD Open Data
description: " "
---

## Here is a collection of data sets relating to IBD, Crohn's Disease, and Ulcerative Colitis. 

Openness and transparency are important, [open data](https://en.wikipedia.org/wiki/Open_data) sets are key to this. Giving people access to data and information helps to allow people to innovate and empowers people to participate in the quest for greater knowledge. 

At the moment I haven't found many data sets. If you have any suggestions for additions, tweet me [@robertshippey](https://twitter.com/robertshippey) or [open an Issue on Github](https://github.com/RobertShippey/IBD-data). In the future I'd like to start researching or collecting new data to include here, but I'm not sure yet what would be valuable, again get in touch with suggestions! 

Sharing is caring. 

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
					<span class="glyphicon glyphicon-{{ post.glyphicon | default: "new-window" }}" aria-hidden="true"></span> Visit</a>
			</div>
		</div>
	</div>

{% cycle ' ', ' ', '</div>' %}

{% endfor %}
