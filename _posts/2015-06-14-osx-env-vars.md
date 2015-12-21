---
layout: post
title: "OSX Environment variables"
date: 2015-06-14 22:53:02 +0100
tags:
 - osx
 - env
---

reference: [http://www.schrodinger.com/kb/1842](http://www.schrodinger.com/kb/1842)

To set an environment variable on Mac OSX, first open a terminal window.

If you are setting the environment variable to run jobs from the command line, use the following command:

{% highlight bash %}
export variable=value
{% endhighlight %}

where variable is the name of the environment variable (such as SCHRODINGER) and value is the value you want to assign to the variable, (such as /opt/schrodinger/suites2013). You can find out which environment variables have been set with the env command.

If you are setting the environment variable globally to use with applications, use the commands given below. The environment variables set by these commands are inherited by any shell or application.

### OS X 10.6, 10.7

To set an environment variable, enter the following command:

{% highlight bash %}
defaults write ~/.MacOSX/environment variable "value"
{% endhighlight %}

To find out which environment variables have been set, enter the following command:

{% highlight bash %}
defaults read ~/.MacOSX/environment
{% endhighlight %}

### OS X 10.8, 10.9, 10.10

To set an environment variable, enter the following command:

{% highlight bash %}
launchctl setenv variable "value"
{% endhighlight %}

To find out if an environment variable is set, use the following command:

{% highlight bash %}
launchctl getenv variable
{% endhighlight %}

To clear an environment variable, use the following command:

{% highlight bash %}
launchctl unsetenv variable
{% endhighlight %}


