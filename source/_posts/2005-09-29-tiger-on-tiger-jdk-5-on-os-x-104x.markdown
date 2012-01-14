---
author: connylundgren
date: '2005-09-29 05:51:41'
layout: post
slug: tiger-on-tiger-jdk-5-on-os-x-104x
status: publish
title: Tiger on Tiger.. (JDK 5 on OS X 10.4.x)
wordpress_id: '22'
categories:
- java
- mac osx
comments: true
---

Apples implementation of JDK 5.0 works terrific, although after installation
1.4.2 is still the default, it easily fixed by some creative symlinking...

    
    
    cd /System/Library/Frameworks/JavaVM.framework/Versions
    mv CurrentJDK CurrentJDK-old
    ln -s 1.5 CurrentJDK

