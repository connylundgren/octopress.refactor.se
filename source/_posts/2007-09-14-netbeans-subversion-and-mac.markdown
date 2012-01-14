---
author: connylundgren
date: '2007-09-14 11:38:10'
layout: post
slug: netbeans-subversion-and-mac
status: publish
title: Netbeans, Subversion and Mac
wordpress_id: '110'
categories:
- ide, netbeans
- mac osx
comments: true
---

NetBeans has SVN support pretty much out-of-the-box, but on OS X you will be
presented with the not so obvious message

> NetBeans Subversion support requires Subversion 1.3 executable!

Install Subversion 1.3 (http://subversion.tigris.org) or later, add it to
PATH, test by running 'svn --version' from command line, and finally restart
IDE, please

  
Since I apparently has forgotten how I made it work before here is the
instruction for future reference, hopefully this will save me (and perhaps
others) from some frustration.

>   1. Fire up a terminal

>   2. Navigate to your Netbeans installtion folder like

**cd /Applications/NetBeans5.5.app/Contents/Resources/NetBeans/bin**

>   3. Open the **netbeans** file in your favorite editor

>   4. On the first line (after comments) add

** PATH=$PATH:/usr/local/bin:/usr/local/sbin  
export PATH**

>   5. Save the file, and restart NetBeans

  
Your all set!

