---
title:  "Open Graph"
date:   2017-11-14 10:17:54 +0100
categories: misc
image: /images/graph3.png
---
Open graph is a technology first introduced by Facebook in 2010. It allows integration between Facebook and other websites by enabling them to become "rich graph objects", with the same functionality as other Facebook objects.

Basically, it allows you to make visible selected pieces of information and data, like images, directly when you create a link to a website in a facebook update. That way, by including a relevant picture and an interesting sentence or two, you could more easily entice readers and subsequently making them click on the link.

In order to make this possible, information is sent via Open Graph meta tags in the <head> part of the website’s code.

## Example

{% highlight javascript linenos %}
{% raw %}
<!-- og:site_name -->
<meta content="{{site.title}}" property="og:site_name">

<!-- og:title -->
{% if page.title %}
  <meta content="{{page.title}}" property="og:title">
{% else %}
  <meta content="{{site.title}}" property="og:title">
{% endif %}

<!-- og:url -->
{% if page.url %}
  <meta content="{{site.url}}{{page.url}}" property="og:url">
{% endif %}

<!-- og:type -->
{% if page.layout == "post" %}
  <meta content="Article" property="og:type">
{% else %}
  <meta content="Page" property="og:type">
{% endif %}

<!-- og:image -->
{% if page.image %}
  <meta content="{{site.url}}{{page.image}}" property="og:image">
{% else %}
  <meta content="{{site.url}}{{site.data.base.img}}" property="og:image">
{% endif %}

<!-- og:description -->
{% if page.excerpt %}
  <meta content="{{page.excerpt | strip_html | truncatewords: 30}}" property="og:description">
{% else %}
  <meta content="{{site.description}}" property="og:description">
{% endif %}
{% endraw %}
{% endhighlight %}

Now, Facebook generally caches your website's Open Graph properties the first time it encounters them, so if you change anything and share your post again, your updated values might not show up. What you need to do is go to [Facebook Sharing Debugger](http://developers.facebook.com/tools/debug){:target="_blank"}, enter the url of your website and request to scrape the URL again simply by pressing a button. Now sharing your post should render just fine!