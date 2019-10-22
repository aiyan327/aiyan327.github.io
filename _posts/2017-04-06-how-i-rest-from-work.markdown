---
layout: post
title: Some Annoying Problems in Setting Up My Blog
date: 2019-10-22 13:32:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: i-rest.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Github Pages, YAML]
---
There are countless articles on instructions of using Github Pages, Jekyll, etc. for people to build their own websites. Forget about Ruby. We noobies don't need that, nor can we properly use it. Check this [website](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/). Even if you closely check every line of the tips and followed every steps, you might still find yourself in a mess. Here's some of my learning from my own mistakes.

## Baseurl
After I forked the Jekyll theme from its repository, my website came out but only with text in blue and white. If you have met this problem too, open your _config.yml file. Find the line of "baseurl:" and add "/(your user name).github.io" to it. Save the change and it should work fine afterwards.

![I and My friends]({{site.baseurl}}/assets/img/we-in-rest.jpg)

## Pictures not showing
After editing the author name and blahblah in my own config.yml, the next thing I tried was to change the profile picture. I added my picture into the "/assets/img" file and changed the author-img (obviously). Then after refreshing the page, there was no picture showing at all.

Then I tried to include the file path ahead of the image file. Still not working.

Finally, I realized that it was because of uppercase/lowercase. My pic was saved as "yan.JPG", but the first time I typed "yan.jpg". Therefore Github cannot recognize it and access to the correct file. Be sure to type everything as you see it.
