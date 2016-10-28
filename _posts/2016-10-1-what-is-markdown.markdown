---
layout: post
title: What is Markdown?
date: 2015-07-15 15:09:00
description: How can I stylize my posts here?
author: Aditi Rajagopal
author_twitter: aditi_rajagopal
---

Markdown text format that allows you to convert plain text to valid HTML. It enables inhabitants of the web to write easy-to-read documentation, code, web pages etc. Here are some easy formatting options: 

Headers & Paragraphs
====================

{% highlight raw  %}

A First Level Header
====================

A Second Level Header
---------------------

### A Third Level Header

This is some paragraph text. 
Just some sample text to fill up some space. 
It's an example. 
Now go forth and write!

{% endhighlight %}

Raw text above will translate to:
<br/>


A First Level Header
====================
<br/>

A Second Level Header
---------------------

### Header 3

<br/>
This is some paragraph text. 

Just some sample text to fill up some space. 

It's an example. 

Now go forth and write!

<br/>

Lists
====

Unordered lists can be formatted like this:

{% highlight raw %}
### When I go to the we16 conference, I'm going to get:
*   Swag.
*   Swag.
*   Swag.
{% endhighlight %}

Which translates to:

### When I go to the we16 conference, I'm going to get:
*   Swag.
*   Swag.
*   Swag.

Ordered lists can be formatted like this:

{% highlight raw %}
###When I go to the we16 conference, I want to learn about:
1. Public Policy
2. Open Source
3. SWE
{% endhighlight %}

Which translates to:

###When I go to the we16 conference, I want to learn about:
1. Public Policy
2. Open Source
3. SWE

Code
====

Would you like to write some code? In this project, we use Pygments for sytanx highlighting. Pygments supports more than 100 languages. Below, is an example in python. All you have to do is wrap your code in a liquid tag: 
{% raw  %}
{% highlight python %}  <br/> code code code <br/> {% endhighlight %}
{% endraw %}

Produces something like this: 

{% highlight python %}

class GetMetrics(object):

    def __init__(self, endpoint, username, password, space_name, org_name):
        self.endpoint = endpoint
        self.username = username
        self.password = password
        self.org_name = org_name
        self.space_name = space_name
        self.access_token, self.space_id = self._fetch_auth_headers()

    def _fetch_auth_headers(self):
        form_data = urllib.urlencode({'user': self.username,
                                      'passwd': self.password,
                                      'space': self.space_name,
                                      'organization': self.org_name})

        login_url = 'https://%s/login' % self.endpoint
        print('Authenticating with [%s] ...' % login_url)
        resp = urllib2.urlopen(url=login_url, data=form_data, timeout=20)

        if resp.getcode() == 200:
            print('[200 OK] Success!')
        else:
            print('There was an error processing your request. :(')
            print('Got HTTP %s' % resp.getcode())

        data = json.loads(resp.read())
        access_token = data["access_token"]
        space_id = data["space_id"]

        return (access_token, space_id)

{% endhighlight %}

Want more markdown? Checkout [this](https://daringfireball.net/projects/markdown/basics) tutorial page for more
