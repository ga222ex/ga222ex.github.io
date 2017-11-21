---
title:  "robots.txt"
date:   2017-11-10 10:17:54 +0100
categories: misc
image: /images/robots.png
---
robots.txt is a textfile that you put in the root directory of your web server. Robots – also known as crawlers or spiders – check this document before crawling a website.

The document consists of one or more colon separated fields, describing to the crawler which parts of the website it is denied permission to crawl. If no such document is found, the entire website is assumed OK to crawl.

Since I want the crawlers to index all pages of my site, I created my robots.txt as such:

User-agent: *

Disallow:

This really doesn’t do anything. It just specifies that the following rules apply to all robots. But since I’m not defining any rules, no part of the website is considered off limits.
Now, it would make sense to disallow certain spambots or other types of malicious bots, perhaps scraping the web for e-mail adresses etc, but unfortunately that doesn’t work. Robots do not have to check robots.txt before scanning a website, and bad robots simply ignore the file.
