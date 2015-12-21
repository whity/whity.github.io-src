---
layout: post
title: "MySQL Dump"
date: 2015-06-18 09:42:32 +0100
tags:
 - mysql
---

Dumping mysql databases using the command **mysqldump**, documentation available in:

- type {% ihighlight bash %} man mysqldump {% endihighlight %} 
- type {% ihighlight bash %} mysqldump --help {% endihighlight %}
- [https://dev.mysql.com/doc/refman/5.5/en/mysqldump.html](https://dev.mysql.com/doc/refman/5.5/en/mysqldump.html)

### Structure

{% highlight bash %}
mysqldump -h [host] -u [username] -p --no-data --databases [databases names]
{% endhighlight %}

### Data

{% highlight bash %}
mysqldump -h [host] -u [username] -p --no-create-info --databases [databases names]
{% endhighlight %}

### Structure and data

{% highlight bash %}
mysqldump -h [host] -u [username] -p --databases [databases names]
{% endhighlight %}

### Specific table(s)

{% highlight bash %}
mysqldump -u [username] -p [database name] [table name] [table name]
{% endhighlight %}
