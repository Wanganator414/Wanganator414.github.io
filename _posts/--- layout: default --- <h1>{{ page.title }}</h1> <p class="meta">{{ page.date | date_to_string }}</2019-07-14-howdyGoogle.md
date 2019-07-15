---
layout: post
title: "༼ つ ◕_◕ ༽つ Howdy Google"
date: 2019-07-14
comments: true
---

Just added some Google Analytics tracking for the site today, now I can see how many times I visit my own site each day (for my own entertainment).

Well, if you plan to do the same for your own Github hosted site, it's free and fairly simple:

1. First go visit [Google Analytics](https://support.google.com/analytics/answer/1008015?hl=en){:target="_blank"} and sign up for an account.

2. Once you're done with account registration there should be an **admin** button at the bottom left corner of your dashboard screen, click on that and head to **Tracking Info**, then **Tracking Code**, copy the code, you will need it later.

3. Now that you have your code, create an html file called ```analytics.html``` in your ```_includes``` folder, paste the code in and save the file. 

(if you don't have an ```_includes``` directory or are not sure what the heck that is, feel free to refer to [this article](https://github.com/barryclark/jekyll-now) on setting up Github Pages with Jeykll)

4. Now go to your ```_layouts``` directory and add ```{%raw%}{% include analytics.html %}{%endraw%}``` inside your ```default.html``` file's ```head``` tags.

Now make sure that all your anti-tracking plugins like Ghostery or adBlock are paused for your site if you want to run a quick test to see if Google is picking up on your site traffic.
