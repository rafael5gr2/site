---
layout: compress
---
<!doctype html>
<html class="no-js" lang="{% if site.language == nil %}en{% else %}{{ site.language }}{% endif %}">
<head>
	{% include head %}
</head>
<body id="top-of-page" class="{{ page.format }}">
	{% include navigation %}

  <div id="masthead">
  	<div class="row">
  		<div class="small-12 columns">
  			<a id="logo" href="{{ site.url }}" title="{{ site.title }} – {{ site.slogan }}">
  				<img src="{{ site.url }}{{ site.baseurl }}/assets/img/{{ site.logo }}" alt="{{ site.title }} – {{ site.slogan }}">
  			</a>
  		</div><!-- /.small-12.columns -->
  	</div><!-- /.row -->
  </div><!-- /#masthead -->

  <div class="masthead-caption">
  	<a href="{{ page.header.caption_url }}">{{ page.header.caption }}</a>
  </div>
  {% elsif page.header.caption %}
  <div class="masthead-caption">
  	{{ page.header.caption }}
  </div>


	{% include footer %}
	{% include footer_scripts %}
</body>
</html>