---
author: connylundgren
date: '2006-11-22 12:44:34'
layout: post
slug: minor-update
status: publish
title: Minor update..
wordpress_id: '74'
categories:
- general
- java
- JSF
- JSR299 (webbeans)
comments: true
---

Well just a quick update what has been going on lately.

### Another certification...

Last week I completed (and cleared) the [Certified JBoss
Developer](http://www.europe.redhat.com/training/jboss_developer.php3), the
test was quite interesting and a good followup to the the JBoss for Advanced
J2EE Developer course I attended a [couple of weeks
back](http://blog.refactor.se/2006/10/21/jboss-training-next-week/). Quite
interesting to write an open-book certification, where you get 24h to complete
the test (taking it at home). I recommend the course to anyone looking for the
nitty-gritty details about JBoss AS (although you can pick up the information
by reading the [JBoss AS
Guide](http://docs.jboss.org/jbossas/jboss4guide/r5/html/)). Although
certification really doesn't tell you anything, it can be a good edge to get
interesting gigs.

### Joined a JSR expert group..

Since I joined the JCP almost 10months ago, I have been more of a lurker (I
haven't participated actively in any JSRs). The time of change is here, some
months ago I requested to join the
[JSR299](http://www.jcp.org/en/jsr/detail?id=299) (WebBeans) expert group, and
yesterday I got the approvement email. The JSR is really interesting, for
those unfamiliar with it it's basically
[Seam](http://www.jboss.com/products/seam) in a standardized way (the JSR is
lead by Gavin King).

### Work, work, work..

It has been real busy week at work (both client wise and internally). My
current project is nearing it's end (implementation wise) and I have had more
time to actually do some coding in the project (ie less meetings, management,
mentoring). I've been concentrating on verifying the overall architecture
against the requirements. Also quite a bit of refactoring, moving out some
common JSF functionalites to reusable components, this have given me a good
chance to really dive into the JSF spec. Hopefully I will make these
components available in some form over the coming months, it's not exactly
rocket-science component but usefully small tidbits.

I have also been busy on weekends, late nights migrating the infrastructure
from old hardware/software to new servers. To this stage we been quite
successfully and we have deprecated some applications, and old hardware. And I
have begun to extend, and introduce a SSO solution to our business critical
applications (most of them homegrown, and on diffent platforms such as .NET,
J2EE, and classic ASP). We settled on [CAS](http://www.ja-
sig.org/products/cas/) which seems to be a proven solution, but we are not
quite there yet. We need to plug this into a Microsoft Active Directory for
the authentication store, any suggestions here are very much welcome.

