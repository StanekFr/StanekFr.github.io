---
layout: post
title: "And yet another py2 vs py3 post"
excerpt: "The link between Legacy Python and polar bears."
image:
  feature: fm-header-6.jpg
modified:
categories:
date: 2016-05-23T00:00:00+00:00
draft: false
comments: true
---

The python 2 vs python 3 conundrum is at the origin of a myriad of
blog posts and angry arguments on the web. I won't repeat the arguments here
(I gathered some links below), but I'll jump
on a deliberately provocative
[post](http://carreau.github.io/posts/planning-an-early-death-for-python-2.html)
by Matthias B., who concluded with the sentence:

*"Remember, Legacy Python is responsible for global warming, encourage people to stay with IE6, and is voting for Donald Trump."*

Of course, this was meant to be a joke. But couldn't Legacy Python *indeed*
be responsible for a little share of global warming?

### Continuous integration and the testing madness

[Travis-CI](https://travis-ci.com/) is a tool which runs your tests for you.
Whenever changes are made to the codebase, Travis-CI builds a test environment
for your project, runs the tests, and warns you if something went wrong.
This process (called "continuous integration") is extremely useful for all
kinds of projects, and is vital for large projects which can't afford to
publish buggy code.

But what does it have to do with py2? Since all major projects are
supporting py2 and py3, they need to run their tests for both versions.
Numpy for example uses
[10 different environments](https://travis-ci.org/numpy/numpy), half of which
is for py2. Each of these is going to need a bit of computational power every
time someone pushes code. Multiply this by the number of projects using
CI and you get a non-negligible amount of CPU time, used only for checking
code compatibility with a legacy version of python.

I wasn't able to find how much resources Travis-CI needs for its services.
Obviously, this is not much in comparison to
[all other resources required to entertain us](http://www.theguardian.com/environment/2015/sep/25/server-data-centre-emissions-air-travel-web-google-facebook-greenhouse-gas)
, but with these kind of arguments we can stop making efforts right now.

So, finally: **yes**, legacy python is hurting polar bears (a little bit).

### Reading

On which side of the flame war are you? Obviously, I am on the [condescending](https://github.com/Carreau/carreau.github.io/issues/4) side (I can afford it: I started using python very late and I have no py2 codebase). However,
py2 support won't last forever ([until 2020](http://www.i-programmer.info/news/216-python/7179-python-27-to-be-maintained-until-2020.html) to be
precise), and the (voluntary) maintainers of several major scientific packages are
about dropping py2
support long before that:

- the [python 3 statement](http://python3statement.github.io/)
- <https://asmeurer.github.io/blog/posts/moving-away-from-python-2/>
- <http://carreau.github.io/posts/20-about-legacy-python-retirement.html>
- the [102.000.000 hits](https://www.google.at/webhp?hl=en#safe=off&hl=en&q=should+I+use+Python+2+or+Python+3)
question on google, and the [official propaganda](https://wiki.python.org/moin/Python2orPython3)
