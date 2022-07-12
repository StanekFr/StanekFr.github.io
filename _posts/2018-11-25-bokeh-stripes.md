---
layout: post
title: "Interactive Warming Stripes"
excerpt: "Simple is beautiful"
image:
  feature: fm-header-6.jpg
modified:
categories:
date: 2018-11-25T00:00:00
draft: false
comments: true
---

You may have encountered the
"[Warming Stripes](https://www.climate-lab-book.ac.uk/2018/warming-stripes/)"
from [Ed Hawkins](http://www.met.reading.ac.uk/~ed/home/index.php),
a beautiful and brilliantly simple visualization of global warming.

I like the purity of the charts, which comes from the absence of labels or
scales. However, this leaves the reader with unanswered
questions, such as *"what is the range of the warming?"* or *"when did the  
warming become so obvious?"*

Therefore, I decided to reproduce the visualizations using
[Bokeh](https://bokeh.pydata.org) and [HoloViews](http://holoviews.org/).
These interactive plots allow to glide your mouse over the chart and
read the values associated with each color:

<iframe src="/images/blog/bokeh-stripes/annual-stripes-700x300.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="300"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

Data: [NASA GISTEMP](https://data.giss.nasa.gov/gistemp/).
Code: on [GitHub](https://github.com/fmaussion/bokeh-stripes).
Larger plot: [here](/images/blog/bokeh-stripes/annual-stripes-1200x600.html).

With the interactivity, more complex plots become possible. Here for example
with monthly anomalies instead of annual values:

<iframe src="/images/blog/bokeh-stripes/monthly-stripes-700x300.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="300"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

Data: [NASA GISTEMP](https://data.giss.nasa.gov/gistemp/).
Code: on [GitHub](https://github.com/fmaussion/bokeh-stripes).
Larger plot: [here](/images/blog/bokeh-stripes/monthly-stripes-1200x600.html).

Feel free to embed these plots wherever you want!
