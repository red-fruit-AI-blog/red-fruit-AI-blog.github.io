---
layout: post
title:  "How to Embed PDF"
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
[link name](/docs/assets/pdf/FILENAME.pdf)
{% endhighlight %}

[Attention is All You Need](/docs/assets/pdf/NIPS-2017-attention-is-all-you-need-Paper.pdf)
