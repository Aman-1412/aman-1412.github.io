---
title: "Converting numbers into words in Excel"
layout: post
date: 2022-08-22 01:00
image: false
headerImage: true
tag:
- excel
- code
- reference
star: false # this turns on the highlight on the blog. 
category: blog
author: aman
description: To convert numbers(Rupees or Dollars) in your excel sheet into their word equivalents
excerpt_separator: <!--more-->
toc: false
---

## What?

A quick blog that contains the script needed for converting numbers into words in your excel sheet

<!--more-->
## TL;DR
{% highlight raw %}
* Open Excel, press Alt+F11
* Go to insert-> Module and paste the script (For USD - get it from the official doc linked below; For INR - use the script shown below)
* Alt+Q, and now you have a function named =SpellNumber(A1) which will convert the number in A1 into words
{% endhighlight %}

## Steps

Follow <a href="https://support.microsoft.com/en-us/office/convert-numbers-into-words-a0d166fb-e1ea-4090-95c8-69442cd55d98">the official guide from microsoft office support</a> to get it working for USD 

To get it working for ₹₹₹ instead of $$$, use this script that I found floating on the internet:

{% gist Aman-1412/835980632428312c8a83239eea6ef8b8 %}

Credits to the original dev, I just changed it a little for my convenience.

_That's all folks!_
