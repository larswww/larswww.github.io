---
layout: post
title:  "Exam Assignment 1 - CSS Preprocessors"
date:   2015-11-26 23:27
categories: webbprogrammerare
comments: true
excerpt: My answers to the questions in the first assignment in the form of my first blogpost
image: assets/sass.jpg
---

> Your blog page should have multiple posts (Swedish or English) and one post where you reflects over the following:

##What do you think of pre-compiling your CSS?

It makes perfect sense for a developer to pre-compile CSS in order to improve efficiency and make maintenance easier. Especially when at the end of it all, it simply outputs a normal CSS file. Which means that
the end result is simple and compatible.

This makes me far more motivated to want to get good at CSS.

##Compare to regular CSS

Coding CSS can feel incredibly repetitive and tedious compared to other types of code. When using a pre-compiler to generate
the CSS you gain some features of modern languages and this makes you more productive. Being able to use variables saved me
a huge amount of time working on this site when i wanted to experiment with the color scheme. Nesting makes really good
sense when you're used to it from other languages, not doing it in normal css feels dumb.

##Which techniques did you use?

When deciding on my color scheme i used set color variables in the main css file and then simply applied an entire
color scheme accross the entire site, all type of tags, classes, everything - by only changing a few variables.

##Pros and cons?

Overall the CSS is easier to work with when developing and maintaining the project. Variables, nesting, mixins and being able
to break up the CSS in several smaller files, but have it ultimately combined into one for speed, is convenient.

Main con is that the CSS you're looking at in the editor will be way different looking from the actual, final file. You might not
recognize your own final CSS, which might be a problem if you want help from someone not using Sass/is familiar with your code.

There's also an initial learning curve of course.

##What do you think of static site generators?

Not needing to rely on installing something like Wordpress or mess around with server configurations is a huge relief. I can now
manage my content in the same interface i use for creating the site in the first place. Saves me learning a new interface.

The experience of editing and generating your site locally is far superior compared vs adding content & editing config in an interface on a server.
WebStorm as an interface is familiar, simple text/FrontMatter is easy to copy when i want similar settings.

The portability of having a clean site that's not dependent on an install on a specific server is good. This makes it easy to
switch hosting when needed and makes freedom of choice for provider easy. Try finding a good WordPress host in China..! Not a problem with a static site.

First-time setup and learning curve is a factor, but i had that with WordPress and its plugins. This feels more universal, granted
we were served a Boilerplate and a Vagrant, not sure how difficult it would be without those, but probably learnable. That being said,
 if you're not a programmer/computer-interested that learning curve might be a bit much for some.

##What type of projects are they suitable for?

Projects that don't require any interaction from a user, or dynamic content. So projects where content will be mostly static once on the site.

##What is robots.txt and how have you configure it for your site?

Robots.txt is a file that most commercial search engines will read. In it you can specify directories or files that shouldn't
be indexed by the search engine, in case there are certain directories/resources you don't want indexed. Or you can specify
for the entire site not to be indexed if you don't want it seen. This is currently my setting.

It's worth noting that it's not mandatory for any search engine to pay attention to your robots.txt file. Whilst the
major engines will, less commercial ones might.

##What is humans.txt and how have you configure it for your site?

Humans.txt is a way to detail who the people behind a certain website is.

##How did you implements comments to blog posts

I created a FrontMatter switch to give me choice of enabling/disabling comments and then pasted the Disqus-provided default
JavaScript include into a Liquid if-statement.

##What is Open Graph and how do you make use of it?

Open Graph is a standard format that some social media sites read in order to present your content correctly when shared on Social Media.
If for instance someone copies the URL to one of your blog entries, then adds the URL in Facebooks share box, how does Facebook know
which image to use, what to put as lead pargraph, title etc? If you've got Open Graph meta tags the social sites that support them
will read them, effectively allowing you control of how your content is presented. (Unless the user edits it on the social media site,
which they may or may not be able to do depending on the site).
