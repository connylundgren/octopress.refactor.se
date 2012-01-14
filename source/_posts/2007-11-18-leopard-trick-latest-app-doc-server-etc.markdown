---
author: connylundgren
date: '2007-11-18 12:41:13'
layout: post
slug: leopard-trick-latest-app-doc-server-etc
status: publish
title: 'Leopard trick: Latest App, doc, server etc.'
wordpress_id: '114'
categories:
- mac
- mac osx
comments: true
---

Just a quick tip for the Leopard users out there, to have a stack in the dock
which reflect you Recent Applications, Recent Documents, Recent Servers,
Favorite Volumes or Favorite Items simply do the following

Fire up a terminal and enter

> defaults write com.apple.dock persistent-others -array-add '{ "tile-data" =
{ "list-type" = 1; }; "tile-type" = "recents-tile"; }'

Followed by a restart of the dock with the trusted

> killall Dock

There should now be a new stack on your dock, change the "mode" by right(ctrl)
clicking the stack to change what the stack shows.

