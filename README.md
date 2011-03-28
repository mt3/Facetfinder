Facetfinder
=============
Facetfinder is a series of wrappers for different search APIs:

- Flickr image search
- Twitter
- Youtube
- Bing news search
- Google blog search
- Delecious tag search

This repository included the flickr, gdata and feedparse module but you should
probably move them to your modules directory

Make sure you have entered your BING & Flickr API keys in Facetfinder.py

### Usage:

	from Facetfinder import Facetfinder

	ff = Facetfinder()

	items = ff.get_blogs('textile')

	for i in items:
		print i.url
		print i.title
		print i.source
		print i.keyword

### Available methods:

	- get_flickr(keyword) #flickr is VERY slow
	- get_twitter(keyword)
	- get_youtube(keyword)
	- get_news(keyword)
	- get_blogs(keyword)
	- get_delicious(keyword)