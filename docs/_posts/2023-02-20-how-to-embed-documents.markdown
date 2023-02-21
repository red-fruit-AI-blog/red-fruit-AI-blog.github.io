---
layout: post
title:  "How to Embed Documents"
date:   2023-02-20 16:16:23 +0800
categories: jekyll create
---

First, place the file in `assets/pdf/` folder. Then, use the following html in the
markdown post:


{% highlight html %}
{% raw %}
<object data="{{ site.url }}{{ site.baseurl }}/assets/pdf/FILENAME.pdf" width="100%" height="1000" type="application/pdf"></object>
{% endraw %}
{% endhighlight %}


<object data="{{ site.url }}{{ site.baseurl }}/assets/pdf/NIPS-2017-attention-is-all-you-need-Paper.pdf" width="100%" height="1000" type="application/pdf"></object>

Alternatively, you can simply provide the link, using:

{% highlight markdown %}
[link name](assets/pdf/FILENAME.pdf)
{% endhighlight %}

[Attention is All You Need](/assets/pdf/NIPS-2017-attention-is-all-you-need-Paper.pdf)

For the link to open in new tab / window, use html syntax to set the `target="_blank"`.

{% highlight html %}
{% raw %}
<a href="{{ site.url }}{{ site.baseurl }}/assets/FILENAME" target="_blank">Yay</a>
{% endraw %}
{% endhighlight %}

<a href="{{ site.url }}{{ site.baseurl }}/assets/html_presentation/presentation.html" target="_blank">Marp Presentation</a>

