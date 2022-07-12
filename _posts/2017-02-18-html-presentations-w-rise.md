---
layout: post
title: "HTML presentations with RISE and Reveal.js"
excerpt: "or: yet another reason to use the jupyter notebook."
image:
  feature: fm-header-6.jpg
modified:
categories:
date: 2017-02-18T09:00:00+01:00
draft: false
comments: true
---

I gave a couple of python workshops at the ACINN recently. It gave me a good
excuse *not* to do what I should do right now, and try two fancy new tools
instead: *Reveal.js* and *RISE*.


### Reveal.js

[Reveal.js](http://lab.hakim.se/reveal-js/) is an open-source tool to create
HTML presentations which will be displayed in an internet browser.
This has a strong advantage: it is platform independent, and displayable on
basically any computer (as opposed to Microsoft Office, which requires an
expensive license). But this alone is maybe not enough to make the tool so
useful: after all, Latex provides similar advantages thanks to its pdf output
(arguably a little bit less fancy though).


### RISE

[RISE](https://github.com/damianavila/RISE) is an open-source tool to convert
jupyter notebooks into *reveal.js* presentations.
Each notebook cell is formatted as a
slide, including title, pictures, bullet lists, and more. In particular,
code snippets *and their output* are displayed in a nice, illustrative way.

Since an example is better than a thousand words, here you go:
[http://fabienmaussion.info/acinn_xarray_workshop](http://fabienmaussion.info/acinn_xarray_workshop)

You can use the arrows in the lower right corner as well as your keyboard to
navigate between slides.
With `escape`, you can trigger an overview of the presentation, illustrating
it's structure into "main slides" and "sub-slides".


### Details

Both tools are quite easy to use after a short familiarization phase. There is
no need to install Reveal.js if you install RISE via conda as suggested
[by their documentation](https://github.com/damianavila/RISE#installation).
After installation, a new button ("Enter/Exit Live Reveal Slideshow") is
available in the notebook toolbar. It is now possible to start presentations
from an active notebook, and even to run code from within the presentation!
Click [here](https://github.com/fmaussion/teaching/blob/master/xarray_intro_acinn/ACINN_workshop_xarray-slides.ipynb)
to have a look at the notebook I wrote to generate the presentation above.
I used the default layout, but there are many ways to personalize
your presentation if you feel like it.

To share your presentation, you can convert your notebook into HTML slides
with the command:

```
 $ jupyter-nbconvert --to slides my-presentation-notebook.ipynb
```

To look at these you'll need a local reveal.js install (see e.g. [here](http://echorand.me/presentation-slides-with-jupyter-notebook.html) for
instructions).

Finally, you can publish your HTML presentations online, too! Either by using
available [online platforms](https://slides.com/explore), or on your own
website like I did. If you use github pages, this can be done
[quite easily](https://cynng.wordpress.com/2014/10/08/using-reveal-js-on-github-pages-for-your-presentations/)
with a few git commands.
