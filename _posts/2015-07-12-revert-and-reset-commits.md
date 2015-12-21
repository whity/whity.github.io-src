---
layout: post
title: "Revert and reset commits"
date: 2015-07-12 23:01:01 +0100
tags:
 - git
---

### reset last commit

{% highlight bash %}
git reset HEAD^
{% endhighlight %}

### revert a specific commit

{% highlight bash %}
git revert [commit]
{% endhighlight %}

### more documentation

- http://git-scm.com/docs/git-reset
- http://git-scm.com/docs/git-revert
