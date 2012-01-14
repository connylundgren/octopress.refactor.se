---
author: connylundgren
date: '2008-09-30 14:23:02'
layout: post
slug: when-is-done-really-done
status: publish
title: When is done really done?
wordpress_id: '135'
categories:
- agile
comments: true
---

I don’t matter if you work agile or in waterfall (or any other "process" for
that matter), one of the most important bits of practice a team (even if you
are coding solo) should get in place is a _Definition Of Done_. The DoD should
be very obvious to everyone involved, and if anyone (including yourself) tries
to stray from the DoD they should be flogged in public (corporate policies may
get in the way here..).

So why is this definition so important? Let us start with an example I
encountered a while ago.

On one of my project there was this developer let us call him "Fred",
initially things were looking ok, he delivered what was promised, and on
inspection the code looked OK (Fred was no wizard, but a fair developer).

Fred got the responsibility to implement a certain part of the project, and
off he went, when asked about the progress there was always a good answer,
like "I’m testing the implementation" or "I found a bug which I am current
fixing". Fred delivered his part of the application, and when integrated they
didn't work. How could that be? We had all seen him write unit-tests? I sat
down and asked Fred what he thought was wrong, and he told me his story. It
turned out he had written a fairly large test suit, but when asked if it has
ever been "working" I got shocked, Fred told me he had never actually run his
test-suite, he had just wrote a whole bunch of test code, but never ever
executed it.

Although this is an extreme case (nonetheless true), it shows how important it
is to have a Definition of what done actually means. We often use the word
done, but rarely define what it actually means.

Is a feature done when it compiles?  When it is integrated?  When it can run
successfully?  When you have 87.3% code coverage?  All of these are possible
interpretations of the same phrase.

It's important for the whole team to have a shared idea of where the finishing
is. Without that some will claim success and other defeat while talking about
the same thing. So where do you begin? First, talk about it; it should be a
collaborative exercise to define it. Most often you will find the ideas
varies, try to at least find a level everyone can agree to, if not you will
easily end up in "almost done" mode again.

