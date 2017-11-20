---
title:  "How I implemented blog comments"
date:   2017-11-13 10:17:54 +0100
categories: blog
image: images/comments.jpg
---
I implemented blog comments on my blog by using Disqus. Disqus is one of the most popular ways to do this, and Disqus alone stands for letting millions of people post more than 50 million comments every month.

Disqus is free to use, but generate revenue through integrated ads. They also provide an ads-free experience, for a monthly subscription. It is avaiable for a wide range of platforms, including such platforms as WordPress, Blogger, Drupal, Joomla, Shopify, and as used on this site, Jekyll.

A more detailed instruction on how to integrate comments is avaiable on the disqus homepage, but in a nutshell, it works like this:

<div class="box">
    <ol>
      <li>Register your site on <a href="https://disqus.com/" target="_blank">Disqus</a>.</li>
      <li>Add a variable called <span class="cursive">comments</span> to the front matter of the blogpost in question and set its value to <span class="cursive">true</span>.</li>
      <li>More to come...</li>
    </ol>
  <p></p>
</div>

<!-- <p>In between a <span class="cursive">{% if page.comments %}</span> and a <span class="cursive">{% endif %}</span> tag, copy and paste a short code snippet in the appropriate template where you'd like Disqus to load.</p> -->


That's it! Happy blogging!