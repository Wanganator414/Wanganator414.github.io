---
layout: post
title: "🌪Custom Weather Widget🌪"
date: 2019-07-26
comments: true
---

👈 Just added a custom weather widget on the left. The UI looks garbage I know, but I tried my best at making one without using bootstrap or templates. 

You may also be wondeirng why I didn't just add a **free, slick, and cleanly made** weather widget for ***FREE*** online. Well, since I'm a complete noob at front end stuff, I might as well start out with something easy like a website widget. The main gist of it consisted of making the crappy UI using `HTML` and `CSS` while adding some finishing touches with a bit of `Java Script`. 

All the source code is freely availble on my [GitHub](https://github.com/Wanganator414/Wanganator414.github.io){:target="_blank"} for critique and usage *(Not saying it's great code, also please change the API keys if you want to try the code)* Now, let's get started.

1. **Design and Style:** This really depends on what you want to have in your widget and your personal taste, I just made mine orange and display a weather icon, the city I want, and the date.

2. **Data Source:** This is where you `GET` *(No pun intended)* all the weather information from, you can either choose to go to a weather website and brute force that information by parsing said website's **DOM**, or you can do it the easy way by using a web **API**.<br><br>An **API**, which stands for *Application Programming Interface*, is a designated method for developers to interact with a certain framework. It can take many forms, such as the **DOM API** where we can acccess `HTML` elements in the **DOM** with `Java Script`'s `document.queryselector()`, or a **web API** where the we the users can interact with the web server to directly aquire website data via `http` requests.<br><br>For this widget, I choose the [Open Weather API](https://openweathermap.org/api){:target="_blank"} through an **API** aggregation service called **Rapid API** where you can have one account and manage requests to multiple databases under that one account. **Open Weather** is a **free API**, that means you can make as many `http` requests to it **free** of charge.

3. **Putting In The Data**: I won't go into detail how to manipulate `HTML` and `CSS` elements via `Java Script` here, so I'll directly talk about the `Java Scipt` code for getting all the weather data. <br><br> <img src="/assets/images/weatherWidgetEx1.png"  title="fetch GET example"> <br><br>All you need to do now is to send a `GET` request to the **API** endpoint provided in the **API** documentation along with the necessary headers and **API key**, and the server should return back a `JSON` object for you to parse and get information from. You can then fill your widget with the returned information however you like.




