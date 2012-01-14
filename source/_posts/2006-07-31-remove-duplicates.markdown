---
author: connylundgren
date: '2006-07-31 21:02:13'
layout: post
slug: remove-duplicates
status: publish
title: Remove duplicates
wordpress_id: '49'
categories:
- java
comments: true
---

I read a [nice post](http://briankuhn.com/?p=47) about removing duplicates
from a list, I must say that im stunned that i didn't think about it. It's so
dead simple.

I post here so I can find it the next time I might need such a little trick :)

public List removeDuplicates(List items) { Set set = new LinkedHashSet();
set.addAll(items); return new ArrayList(set); }

