---
author: connylundgren
date: '2006-07-19 13:33:46'
layout: post
slug: sun-jdk-on-ubuntu-the-multiverse-way
status: publish
title: Sun JDK on Ubuntu (The multiverse way)
wordpress_id: '48'
categories:
- java
- linux
comments: true
---

The 6.06 Dapper release includes support for Sun JVMs via the Multiverse
repositories. Add support for multiverse to your **/etc/apt/sources.list**

> deb http://pa.archive.ubuntu.com/ubuntu/ dapper multiverse deb-src
http://pa.archive.ubuntu.com/ubuntu/ dapper multiverse

Do a standard **sudo apt-get update** , followed by a **sudo apt-get install
sun-java5-jdk** .

