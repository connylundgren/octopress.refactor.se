---
author: connylundgren
date: '2007-04-02 19:28:13'
layout: post
slug: weblogic-10-on-os-x
status: publish
title: Weblogic 10 on OS X..
wordpress_id: '102'
categories:
- java
- mac osx
comments: true
---

Weblogic, being one of the major player in the Java EE app server space [relea
sed](http://www.bea.com/framework.jsp?CNT=pr01796.htm&FP=/content/news_events/
press_releases/2007) the first fully
[certified](http://java.sun.com/javaee/overview/compatibility.jsp) final
release last week (although a fully certified tech preview has been available
for a while now.).

Being a longtime Weblogic user (my current project using Weblogic 9.2 to name
just one) I decided to give it a spin. Since BEA doesn't support OS X I start
out by making the beast run on my preferred platform, fortunately its quite
easy, and I have previously blogged about it. So here is a quick recap for
WLS10.

Firstly [download](http://commerce.bea.com/showproduct.jsp?family=WLS&major=10
&minor=0) the HP-UX Itanium release (_server100_generic.jar_)

Start the graphical installer by running

> java -Dos.name=unix -jar server100_generic.jar

One installed, go ahead and create a new domain (or upgrade an existing if
thats your game), use the **_wlserver_10.0/common/bin/config.sh_** to start
the wizard.

Voila, your ready to go. Start the new domain and start playing around with
WLS10.

And of course, running Weblogic on OSX is not supported by BEA in any way.

My next step is to evaluate the WLS10, to get to know it a bit better. Ill
take a existing Java EE app and make it run on WLS 10 (The app is currently in
production on JBoss AS, and I've previously "ported" it to Glassfish). So hand
around for my observations. _ Note, by using this approach you will miss out
on the platform dependent optimization (namely using native libraries, but
this method has served me good in the past)._

to be continued...

**Update:** It has come to my attention that the console may freeze (and the CPU jumps to 100%) when trying to login to the console (I didn't run into it since I had made theese changes anyway). Change/add the following to _bin/setDomainEnv.sh _

> USER_MEM_ARGS="-Xms512m -Xmx1024m -XX:MaxPermSize=128m"

