---
layout: post
title: "Bokeh viz: Glacier evolution in the Alps"
excerpt: "A simple line plot can take some time"
image:
  feature: fm-header-6.jpg
modified:
categories:
date: 2019-12-05T00:00:00
draft: false
comments: true
---

In a recent study, [Zekollari et al. (2019)](https://www.the-cryosphere.net/13/1125/2019/),
computed the predicted volume change of all glaciers in the European Alps.

We display these data in the interactive plot below.
It shows the future evolution of Alpine glaciers' volume under various
emission scenarios, and for selected countries/regions. Glacier change
is displayed in % of their estimated volume in 2017. When hovering
with the mouse over each curve, you can display the data in plain text,
**as well as the estimated uncertainty** (±σ, indicating
that there is an estimated 68% probability that the actual future glacier
volume will fall within that range).

<iframe src="/images/blog/bokeh-alps/alps_future.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="300"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

Data: [Zekollari et al. (2019)](https://www.the-cryosphere.net/13/1125/2019/).
Code: on [GitHub](https://gist.github.com/fmaussion/2ce2496774639f16f8c5bddeece3473a).
Larger plot: [here](/images/blog/bokeh-alps/alps_future_large.html).


Thanks to the [HoloViews](http://holoviews.org/) library for the great tools!
