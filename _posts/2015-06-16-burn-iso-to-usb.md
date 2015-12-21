---
layout: post
title: "Burn iso image to usb on OSX"
date: 2015-06-16 09:56:00 +0100
tags:
 - osx
 - iso
 - usb
---

- open 'Disk utility' to unmount usb partition
- check usb partition

    {% highlight bash %}
    diskutil list
    {% endhighlight %}
- burn iso to usb

    {% highlight bash %}
    sudo dd if=DISK-IMAGE.iso of=/dev/DRIVE-NAME
    {% endhighlight %}
