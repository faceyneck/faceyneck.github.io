---
layout: post
title: "Web Development is Virtually AIDS"
categories: Rants
permalink: "/web-development-is-virtually-aids/"
---

This website was built using Jekyll, and although it's probably an elegant piece of software, I fuckin' hate it.

I don't hate Jekyll as though it's somehow worse than other web technologies out there; instead I hate it because it _is_ a web technology.

This website has been a non-stop headache from the very beginning. Is that unique to web development in general?

# FUCK NO!

Here's a wonderful example of the kinds of bull shit one encounters when doing web development. (Referred to extensively in my friend's cirles as "webshit.")

Here's a snippet of code from YouTube, if you wanted to embed a video on your Jekyll website:

{% highlight html %}

<iframe width="933" height="527" src="https://www.youtube.com/embed/fwMukKqx-Os" title="George Carlin  About Rape" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

{% endhighlight %}

That's for a George Carlin video that I was discussing in another post.

# IT DOESN'T WORK

**Here** is the snippet of YouTube embed code that _does_ work:

{% highlight html %}

<iframe width="933" height="527" src="https://www.youtube.com/embed/fwMukKqx-Os" title="George Carlin  About Rape" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen> </iframe>

{% endhighlight %}

See the difference?

Probably not.

If you're embedding ***one*** video on your web page, it's all hunky-fucking-dory. If you embed ***two*** videos, everything goes to shit. Jekyll will generate the webpage with whatever the first video was twice, and the 2nd video you were trying to embed on your webpage won't show.

Here's the sole difference that makes all of the... well... difference.

First, the code snippet that doesn't work:
{% highlight html %}

<iframe width="933"...allowfullscreen></iframe>

{% endhighlight %}

...and now the one that does:

{% highlight html %}

<iframe width="933"...allowfullscreen> </iframe>

{% endhighlight %}

The _only_ difference is one space. _**ONE FUCKING SPACE MAKES ALL THE FUCKING DIFFERENCE GOD FUCKING FUCK**_.

This entire website has been one stupid issue after the other. Or, in other words:

# WEB DEVELOPMENT IS VIRTUALLY AIDS