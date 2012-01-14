---
author: connylundgren
date: '2006-03-28 23:15:22'
layout: post
slug: weblogic-91-on-os-x
status: publish
title: Weblogic 9.1 on OS X
wordpress_id: '23'
categories:
- java
- mac osx
comments: true
---

I've had WLS 8.1 running on my PowerBook lately, using the
[tips](http://www.oreillynet.com/pub/wlg/4091) posted Rod Chavez. That
installation required some tweaking to get it to work properly.

Since my current project will probably move to a WLS 9 before going into
production, I would like to get WLS9 running on my PowerBook (although I use
the client supplied Wintel box for onsite development), the opportunity to
work while waiting for the delayed flight home is quite appealing.

After some digging it seams like the installer is quite OS agnostic, and I
takes a os argument when running the installer. The tip here is to use the
switch '-Dos.name=unix'.

> java -Dos.name=unix -jar server910_generic.jar

![](http://blog.refactor.se/static/wls9_1.png)

_installer stating_

![](http://blog.refactor.se/static/wls9_2.png)

_done installing_

![](http://blog.refactor.se/static/wls9_3.png)

_quickstart_

run

> /BEA_HOME/weblogic1/common/bin/conf.py

to start the config wizard.

  
**note, running WLS is not "officially" supported by BEA. But in my experience it works like a charm..**

