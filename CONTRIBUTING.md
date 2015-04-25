Contributing
============

Welcome to the OSU Security Club Website!  This site is powered 
by Jekyll and hosted on Github.  

Mechanics
~~~~~~~~~

First Things First
------------------

1. Fork the repository
2. Clone it
3. Checkout your own branch ``$ git checkout -b <USERNAME>/contrib``

Using Jekyll
------------

1. Installing Jekyll is very easy: ``$ gem install jekyll``. If you have any problems, check out [the Jekyll website](http://jekyllrb.com/)
2. In the root of the website (same directory as ``_config.yml``), run ``$ jekyll serve``
3. Visit 127.0.0.1:4000 to see the site! It updates live as you make your changes, so no need to keep rebuilding.

Committing and Pushing
----------------------

Once you've made all the changes you'd like run 
1. ``$ git status``
2. ``$ git add <FILE>`` all of the files you changed.  
3. Commit your changes ``$ git commit`` and enter a helpful commit message describing what you did.
4. Push to your branch ``$ git push origin <branchname>``
5. Go to https://github.com/osusec/osusec.github.io and click the big green button. You want to compare master to the branch you just pushed to.
6. Create a pull request, but don't merge it!  We will look over your pull request as soon as we can and see if we can merge it.
7. Profit.

File Structure
~~~~~~~~~~~~~~

The file structure may seem a little unintuitive if you haven't used
Jekyll before, so let me clarify things a little.  

About Page and Meeting Notes
----------------------------
The about page
and meeting-notes page require some templating, so they are in their
own directories.  This is both so they are easy to find, and so that
their urls are pretty (ie http://url.com/about/).  If you are 
interested in modifying them, both of them are html pages which use
/layouts/default.html as their template.   The 
people directory contains biography of all of the officers, which
gets compiled into the about page, and the events directory contains
all of the events which get thrown onto the index page.  These need
to be prepended with a date (any date) according to Jekyll law; I 
don't like it either, it's just how it is.  There are template 
pages in both of these directories that can help you get started adding
a new person or event.  


Layouts Directory
-----------------
The layouts directory
contains, well, layouts (or templates) that other pages use. For 
instance, all of the pages with "layout: post" use ``layouts/post.html``
page as their template, injecting things like title and content 
into the variables on the ``layouts/post.html`` page. 

Assets
------
The assets directory contains css and images.  Link to it using 
``assets/<filepath to thing>``

_posts
------
This is where Resources and Code of Ethics pages live.  They are
"normal" pages that don't require special html like about and 
meeting notes.  They're written in [markdown](http://daringfireball.net/projects/markdown/),
and then compiled into html.  

Site
----
This is the directory the site gets built into.  Don't touch it. 
Please.


