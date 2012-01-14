---
author: connylundgren
date: '2005-12-20 12:57:25'
layout: post
slug: the-voes-of-multi-ide-projects
status: publish
title: The voes of multi-IDE projects.
wordpress_id: '10'
categories:
- general
comments: true
---

At my current gig we use multiple IDE's for different tasks (of historic
reasons as well as pure productive reasons). Today the team uses Borland
JBuilder, Intellij IDEA and Eclipse.

The suggested/preferred choice is JBuilder, but the project has decided to be
IDE independent, and today JBuilder is almost exclusively used by the EJB-
developers (team is split between EJB, Web/Frontend and
Persistence/Hibernate). The Hibernate Team uses Eclipse, since it makes a lot
of sense to use some of the rich plugins available for this IDE.

The project has a directory structucture set up, an ant file for
building/deploying etc. The problem is that JBuilder seems to spread a lot of
files around the whole repository, ad hoc META-INF directories, .class files
in strange places and some other arbitrary files.

I must say that I am no JBuilder fan, but it has some really nice features for
those not that into "code" (i.e. WYSIWYG/Code generation for e.g. EJB's). But
I highly dislike it spreading it's files all around it, as said before Eclipse
& IDEA has no problem with a predefined directory structure, but JBuilder
really insist on rolling it's own, highly annoying. For the time being I
believe I got it under control by hacking strange JBuilder xml-files, and
heavy usage of .cvsignore .. I only wish it were easier.

