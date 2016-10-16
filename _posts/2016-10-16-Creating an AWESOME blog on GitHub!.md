---
layout: post
title: Creating an AWESOME blog on GitHub!
---

Hello! Well it's my first post, so I hope it will introduce you gently into my writing style. Writing posts is a big challenge for software engineers, which are more programming oriented people. Let me present you blogging from technical side. 

<!--more-->

GitHub Pages
------------

Hosting is very important aspect of blog creation. There are many ways of how to host a website. I present you, very elegant solution presented by GitHub. [GitHub Pages](https://pages.github.com/) is simple solution allowing programmers create their website just by creating GitHub repository. Is it really so simple? Yes, all you need to do is create repository with name **`username.github.io`**, then push a commit with your page content. Now you can visit your website at **`username.github.io`**. You're welcome! :)

Jekyll
------------

[Jekyll](https://jekyllrb.com/) is technology fully supported by GitHub Pages, which provides static website from plain text. Instalation of Jekyll is a simple process. All you need to do is type: 

**`gem install jekyll bundler`**

Now if you want to create new page:

**`jekyll new my-page-name`**

To run your website just type:

 **`bundle exec jekyll serve `**


By default your website will be available at [localhost:4000](localhost:4000).
Jekyll is providing [great documentation](https://jekyllrb.com/docs/home/), which describes whole blog creation step by step.

Templates are awesome!
------------

Do you know what is more awesome than templates? CSS! 

<img src="{{ '/assets/img/css.png' | prepend: site.baseurl }}"> 

Seriously, there is nothing more irritating than fighting with design of your website (from my point of view). Jekyll templates come us with help, there are plenty of Jekyll templates and them are truly awesome. [Check them out](http://lmgtfy.com/?q=jekyll+templates).

First post
------------

Writing the first post is always a problem, thinking about a subject of post and writing a content is the hardest part. There is no golden receipt for this, but we can focus on how to do create first post in Jekyll. First you need to go to folder with content of your website and create new file in directory named **`_posts`**. File name should match pattern **`YYYY-MM-DD-title.extension`**. Jekyll is supporting many of known extensions like html, markdown or textfile. The content of the post should look like this:

{% highlight text %}---
layout: post
title: Creating an AWESOME blog on GitHub!
---

Hello! Well it's my first post, so I hope it will introduce you gently...{% endhighlight %}

You can see that we need a special part of top of the file, called front matter, where you can specify metadata of post. Like layout, title, excerpt separator and so on. Then you can start writing your content of website.

That's all folks. :)