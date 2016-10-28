#we16 Open Sourced

This is a sample blog that will be used to collect ideas, posts, images, and more from the 2016 Society of Women Engineers annual conference.

Features
--------

Blog Posts
==========

Add a post if you'd like. Just ask to join the group, and create a pull request (PR)

Lists
=====

Add a list, or add on to the existing lists. Both via a PR

Beginners: How to Contribute a ReadMe
-------------------------------------

1. Go to the we16 open source repository (If you don’t have a GitHub account yet, you can create one in about 2 minutes.)
2. Click the “New File” button. This will automatically create a fork (your own personal copy) of the repository.
3. Name your file “-readme.md” (the “md” stands for Markdown, a popular alternative to plain .txt files).
4. Type out your article. If you’re unfamiliar with Markdown, you can write your article here, then copy and paste it onto GitHub.
5. Scroll down and fill in a commit message (for example, “Created a readme that introduces me as a new contributor”) and add a description. If you’re writing this article in response to an article request (see the issues tab), you should reference it in the description like so: “Closes issue #177.”
6. Click “Propose new file.”
7. Click “Create pull request.” Your pull request will already be populated from your commit message and description. So click “Create pull request” again to finalize it.

Specifics
=========

You can add an additional post or list by creating a new file in the respective _post or _list directories, and filling out the YAML front matter below:

---
layout: post
title:  Title of your post
date: 2015-10-27 23:45:00 //YEAR-MONTH-DAY HOUR:MINUTE:SECONDS
description: An excerpt or description of the post
author: Your name
author_twitter: Your twitter handle minus the '@'
---

Use the existing posts as an example. The easiest way to do this is to copy and paste the contents of an existing post and editing it

Photos
======

Photo formatting is made simple using rows of a 3-column system. Make photos 1/3, 2/3, or full width. Easily create beautiful grids within your blog posts and projects pages.

Code Highlighting
=================

This theme implements Jekyll's built in code syntax highlighting with Pygments. Just use a liquid tag to delineate your code: {% highlight python %} code code code {% endhighlight %}



The MIT License (MIT) Copyright (c) 2016 Aditi Rajagopal

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.