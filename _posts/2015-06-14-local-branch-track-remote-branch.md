---
layout: post
title: "Local branch track remote branch"
date: 2015-06-14 22:48:07 +0100
tags:
 - git
---

### As of Git 1.8.0

{% highlight bash %}
git branch -u upstream/foo
{% endhighlight %}

Or, if local branch foo is not the current branch:

{% highlight bash %}
git branch -u upstream/foo foo
{% endhighlight %}

Or, if you like to type longer commands, these are equivalent to the above two:

{% highlight bash %}
git branch --set-upstream-to=upstream/foo
git branch --set-upstream-to=upstream/foo foo
{% endhighlight %}

### As of Git 1.7.0

{% highlight bash %}
git branch --set-upstream foo upstream/foo
{% endhighlight %}
