---
_schema: default
date: 2024-12-23
title: Converting XML Catalogs to TR9401 Catalogs
post_permalink: /blog/{{ title | slugify }}/
seo:
  page_description: 
  canonical_url: 
  featured_image: 
  author_twitter_handle:
  open_graph_type: article
  no_index: false
layout: layouts/blog-single.liquid
tags:
  - XML Catalogs
  - TR9401 Catalogs 
  - XSLT Conversion
author: Earl Hood, Senior Computer Systems Designer at EPS Corporation
thumbImg:
  image: https://picsum.photos/id/363/200/300
  image_alt: Electric train yard with a myriad of overhead lines and tracks on the ground. An electric train sits facing the camera in the lower left of the frame. Photo (c) José Martín.
featuredImg:
  image: https://picsum.photos/id/363/200/300
  image_alt: Electric train yard with a myriad of overhead lines and tracks on the ground. An electric train sits facing the camera in the lower left of the frame. Photo (c) José Martín.
draft: false
---

<h2>Converting XML Catalogs to TR9401 Catalogs</h2>

I have been working with SGML/XML for some time now and have come across software that does not support [XML Catalogs](https://xmlcatalogs.org/), including software that I developed. 

However, this software does support [TR9401 Catalogs](https://www.oasis-open.org/specs/a401.htm). Instead of trying to update or modify older software, I have found it easier to write an XSLT that converts an XML Catalog into a TR9401 catalog. 

You can view and download the XSLT from:

[xmlcat-to-opencat.xsl](http://www.earlhood.com/blogspot/files/xmlcat-to-opencat.xsl)

If there are any features in the XML Catalogs that are not supported in TR9401, the XSLT displays warnings but continues processing. 

Although I'm unsure if anyone else would find this transformation useful, it has proven handy for me when using my old DTD parsing tools.

<h3>Additional Resources</h3>
* [Entity Management @ Oasis-open.org](https://www.oasis-open.org/specs/a401.htm)
* [XML Catalogs page @ xmlcatalogs.org](https://xmlcatalogs.org/)
* XMLCat-to-OpenCat.xhml @ earlhood.com](http://www.earlhood.com/blogspot/files/xmlcat-to-opencat.xsl)
