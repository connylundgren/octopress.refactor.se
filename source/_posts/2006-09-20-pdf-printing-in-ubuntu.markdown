---
author: connylundgren
date: '2006-09-20 07:59:14'
layout: post
slug: pdf-printing-in-ubuntu
status: publish
title: PDF Printing in Ubuntu
wordpress_id: '64'
categories:
- linux
- ubuntu
comments: true
---

One of the nicest features on my OSX machine is the built in function to print
everything to a PDF, fortunate it's really easy to ad this feature to Ubuntu
to (for the record when forced to used a Windows box the free
ware&nbsp_place_holder;[PrimoPDF](http://www.primopdf.com/) does a decent job
as-well)

Start of by installing the **cups-pdf** package with apt (or synaptic if you
prefer).

>

**sudo apt-get install cups-pdf  
**

Next do a

>

**sudo chmod +s /usr/lib/cups/backend/cups-pdf**

Finally in Gnome add a new printer by going to “**System > Administration >
Printing**”, select New Printer select Local Printer & Use a Detached Printer,
select PDF Printer.

Onto the next screen select the Generic manufacturer, and the “**Postscript
color printer rev3b**”. Leave the driver set to “**Standard**”

You are now up and running with PDF printing in Ubuntu.

By default the PDF-files is stored in **~/PDF** , but this is easily changed
by modifying your** /etc/cups/cups-pdf.conf** look for the line **Out
${HOME}/PDF**

