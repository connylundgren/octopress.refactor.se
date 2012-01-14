---
author: connylundgren
date: '2006-02-13 20:49:30'
layout: post
slug: manifestmf-classpath-from-ant
status: publish
title: MANIFEST.MF Classpath from ANT
wordpress_id: '30'
categories:
- java
comments: true
---

Although unsupported, it is possible to create dependencies in MANIFEST.MF
files in the format

> Class-Path: lib/hibernate3.jar lib/log4j.jar

On the gig i currently work in we have all our 3rd party libs (jar-files) in a
structure like this lib/hibernate-3.0.5. To generate the manifest by hand is
not optimal, so we would like ANT to generate the manifest automatically. We
use ant 1.6.2, and I believe a 1.6 should be a minimum to use this hack This
is how we solved the problem

  1. First of, define the properties
  2. Next of, modify you jar-making target. This is were the "hack" is, we store all the depenncies in a temp variable (dep.libs)[source:XML]<pathconvert property="dep.libs" pathsep=" "> <mapper> <chainedmapper> <!-- remove the full path --> <flattenmapper /> <!-- prefix every .jar with lib/ --> <globmapper from="*" to="lib/*" /> </chainedmapper> </mapper>  
<path> <fileset dir="${lib.dir}"> <include name="**/*.jar" /> </fileset>
</path> </pathconvert>

<!-- create the actual jar --> <jar jarfile="${build.dir}/myjar.jar"
basedir="${build.dir}/classes"> <manifest> <!-- other manifest details goes
here --> <!-- insert our formated libs --> <attribute name="Class-Path"
value="${dep.libs}" /> </manifest> </jar> </target> [/source]

