---
layout: post
title: "Comment Time"
date: 2019-07-14
---
Almost done finalizing everything for the site, just added a neat little Disqus comment section (that hopefully is displayed at the bottom).

Making it work wasn't too bad:

1. First head over to [Disqus](https://disqus.com) and get a free subscription and follow the steps for your specific site hosting platform.

2. For Jekyll, follow the Jekyll tutorial and remember to copy the universal embed code from the disqus site.

3. Take the embed code and make an html file in your github site's **_includes** folder.

4. Edit the embed code according to the comment hints and save it.

5. Go to your **_layouts** folder and add ```{% include disqus.html %}```	right under ```{{content}}``` in your **post.html** file (or within a <div> tag).

Make sure your blog posts are using the **post** layout instead of the **default** layout in the setup area and you should be good to go.
