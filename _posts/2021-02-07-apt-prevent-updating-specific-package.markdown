---
title: "apt prevent updating a specific package"
layout: post
date: 2021-02-07 13:10
image: /assets/images/2-apt-hold/apt-package-manager.png
headerImage: true
tag:
- linux
- ubuntu
- apt
star: false # this turns on the highlight on the blog. 
category: blog
author: aman
description: Prevent packages from upgrading via apt
excerpt_separator: <!--more-->
---

<span class="evidence">
(**Note:** This is not the first blog. The first blog has been hidden, I'll upload it once I've finalized it.)
</span>

Ever had a need to prevent particular troublesome packages from being upgraded? (Looking at you virtualbox)

<!--more-->

---

You can easily hold back particular package from being upgraded by using the `apt-mark` command.

{% highlight sh %}
$ sudo apt-mark hold virtualbox-6.1
{% endhighlight %}


And that's it!

<!-- ![apt-mark hold]({{ site.url }}/assets/images/2-apt-hold/apt-mark-hold.png) -->
<img src="{{ site.url }}/assets/images/2-apt-hold/apt-mark-hold.png" alt="apt-mark-hold" width="336px" height="56px" loading="lazy">
<figcaption class="caption">apt-mark hold</figcaption>


Now, when you run `sudo apt upgrade`, it won't ugrade your package(virtualbox in my case)   


<!-- ![sudo apt upgrade]({{ site.url }}/assets/images/2-apt-hold/virtualbox-not-upgraded.png) -->
<img src="{{ site.url }}/assets/images/2-apt-hold/virtualbox-not-upgraded.png" alt="sudo apt upgrade" width="727px" height="292px" loading="lazy">
<figcaption class="caption">sudo apt upgrade</figcaption>


If you want to see all the packages that are being held back, you can run:

{% highlight sh %}
$ apt-mark showhold
{% endhighlight %}


<!-- ![apt-mark showhold]({{ site.url }}/assets/images/2-apt-hold/apt-mark-showhold.png) -->
<img src="{{ site.url }}/assets/images/2-apt-hold/apt-mark-showhold.png" alt="apt-mark showhold" width="205px" height="57px" loading="lazy">
<figcaption class="caption">apt-mark showhold</figcaption>



To unhold the package, simply run:

{% highlight sh %}
$ sudo apt-mark unhold virtualbox-6.1
{% endhighlight %}


<!-- ![apt-mark unhold]({{ site.url }}/assets/images/2-apt-hold/apt-mark-unhold.png) -->
<img src="{{ site.url }}/assets/images/2-apt-hold/apt-mark-unhold.png" alt="apt-mark unhold" width="397px" height="147px" loading="lazy">
<figcaption class="caption">apt-mark unhold</figcaption>


That's all folks!


**References:**

- <https://manpages.ubuntu.com/manpages/bionic/man8/apt-mark.8.html/>
- <https://askubuntu.com/questions/18654/how-to-prevent-updating-of-a-specific-package/>