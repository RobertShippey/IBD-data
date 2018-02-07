---
layout: layout
title: IBD Open Data
description: " "
---

## Here is a collection of data sets relating to IBD, Crohn's Disease and Ulcerative Colitis. 

Openness and transparency are important, [open data](https://en.wikipedia.org/wiki/Open_data) sets are key to this. Giving people access to data and information helps to allow people to innovate and empowers people to participate in the quest for greater knowledge. 

At the moment I haven't found many data sets. If you have any suggestions for additions, tweet me [@robertshippey](https://twitter.com/robertshippey) or [open an Issue on Github](https://github.com/RobertShippey/IBD-data). In the future I'd like to start researching or collecting new data to include here, but I'm not sure yet what would be valuable, again get in touch with suggestions! 

Sharing is caring. 

<div class="row">

{% for post in site.posts %}

	<div class="col-sm-6 col-md-4 float-block-left">
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

{% endfor %}

</div>
<div class="clearfix"></div>

<hr>

<h4>Privacy, copyright and stuff</h4>

I don't use any tracking or data collection software here. 

I've embedded the Twitter Widget and although I've enabled their 'Do Not Track' option for that, they'll probably still be collecting data and setting cookies for you. You can see <a href="https://dev.twitter.com/web/overview/privacy">Twitter's info on widget privacy here</a>. 

I've hosted this on GitHub Pages and as far as I can see they don't track any information, but see <a href="https://help.github.com/articles/github-privacy-statement/">GitHub's Privacy Statement</a> for more info. 

I don't own the copyright to any of the datasets here. I've used some of their own text to explain the data for simplicity, I hope that's okay. 

I'll never accept any payments of gifts in exchange for inclusion on this page. 

Contact me, <a href="https://twitter.com/robertshipey">Robert Shippey</a>, if you have any questions or concerns. 

The site itself: This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
