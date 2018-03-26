# Index

## Liste des posts 
<ul>
	{% for post in site.posts %}
	<li>
		<a href="{{ post.url }}">{{ post.title }}</a>
	</li>
	{% endfor %}
</ul>

## Liste des customFiles

<ul>
	{% assign custom_files = site.static_files | where: "customFile", true %}
	{% for file in custom_files %}
	<li>
		<a href="{{ file.path }}">{{ file.basename }}</a>
	</li>
	{% endfor %}
</ul>

## Liste des static_files
<ul>
	{% for file in site.static_files %}
	<li>
		{{ file.path }}
	</li>
	{% endfor %}
</ul>
