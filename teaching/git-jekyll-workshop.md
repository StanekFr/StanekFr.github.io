---
layout: page
image:
  feature: fm-header-4.jpg
title: "Workshop: create your own website with jekyll and github-pages"
modified: 2018-05-29
---

A nice and engaging website is a strong asset for your future job search.
Fortunately, it is nowadays quite easy to make websites without much knowledge
about HTML or JavaScript thanks to so-called [static site generators](https://learn.cloudcannon.com/jekyll/why-use-a-static-site-generator/).
They require a little more technical background than web-based content management
systems like WordPress, but they are also much more lightweight and easier
to handle (in my opinion). Furthermore, they allow to learn another important
tool for scientists: the version control system [git](https://git-scm.com/).

Here are some example of static websites generated with [Jekyll](https://jekyllrb.com)
and hosted on [github pages](https://pages.github.com/):

- a personal website: [fabienmaussion.info](http://fabienmaussion.info/)
- a project website: [oggm.org](http://oggm.org/)
- an educational website: [transparency-lecture.github.io](https://transparency-lecture.github.io/])


In this **first workshop** (beginner level, about 3hrs), we are going to learn:

- how to create a website on github pages
- how to maintain it using git+github
- how to apply the git+github/gitlab workflow to your other personal projects
  (like your programming code or your paper drafts)

In the **second workshop** (intermediate level, about 3hrs), we are going to learn:

- how to use git+github/gitlab for collaborative work
- how the work on major open source packages is coordinated on github
- how to contribute to open source packages

The two workshops are related but it is possible to assist to only one of them
as well. Please be aware that a minimum working knowledge of a command line
(or the willingness to use it) is a prerequisite for using both git and jekyll.
The second workshop assumes that you already have some basic knowledge about
git (e.g. obtained from the first workshop).


## Presentation (Workshop 1)

The slides of the first presentation are available [here](http://fabienmaussion.info/git-jekyll-ws/).

## Presentation (Workshop 2)

The slides of the second presentation are available [here](http://fabienmaussion.info/git-intermediate-ws/).


## Installation instructions (Workshop 1)

If you wish to actively participate during the workshop (highly recommended,
regardless if you wish to create a website or not), you will have to bring
your own laptop and install git and jekyll prior to the event.
Both tools are fairly easy to install and should
work on all three major operating systems (Windows/Mac/Linux).

**Alternatively**, you will be able to use the university computers in the
EDV room. If you haven't done so already,
[request a linux account](https://orawww.uibk.ac.at/public_prod/owa/uvw$web$10.p001)
at ZID.


### Installing git

To install git, follow the instructions from the official website:
[https://git-scm.com/downloads](https://git-scm.com/downloads)

Once installed, you can check your installation by opening a terminal (on
Windows, I recommend to use the newly installed ``Git Bash`` program which
should be available in your windows "Start" menu) and type:

    git --version

If the git software version shows up without error, you should be good to go.

### Installing Jekyll

Installing Jekyll should be fairly straightforward as well. Follow the
instructions for your OS as described on the official website:
[https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/)

IF everything went well, you should be able to open a terminal (on windows:
``Git Bash``) and type:

    jekyll -v

If the software version shows up without error, you should be able to run the
following command, which will create a new website folder in the current
directory:

    jekyll new jekyll-website


### Installing Jekyll on your university account

Start a Linux instance. In the terminal, run:

    $ module avail
    $ module load ruby/2.5.1

Now you should have a more recent version of Ruby available. You should *always*
run the two commands above before using Jekyll. The rest of the procedure is
as simple as described on the
[install Jekyll for Ubuntu documentation](https://jekyllrb.com/docs/installation/#ubuntu).

### Optional: creating a github account

If you plan to host your webpage on [github pages](https://pages.github.com/)
(free) or if you plan to use github for opersonal or open source projects,
I recommend to create a [github account](https://github.com/join).
Personally, I run my github account [under my real name](https://github.com/fmaussion)
and affiliation, because I consider github to be a professional platform and an extension
of my CV.

Using github is not *necessary* in order to take full advantage of git.
As will be discussed during the  workshop, there are alternative platforms such
as the [UIBK Gitlab](https://git.uibk.ac.at). Similarly, there
are alternatives to [github pages](https://pages.github.com/) for hosting your
webpage, even if github pages is probably the most convenient.
