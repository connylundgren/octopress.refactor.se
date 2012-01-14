---
author: connylundgren
date: '2007-01-02 18:01:30'
layout: post
slug: mounting-mac-idisk-on-ubuntu
status: publish
title: Mounting .mac iDisk on Ubuntu
wordpress_id: '85'
categories:
- linux
- mac osx
- ubuntu
comments: true
---

I tend to keep some files that I need access to from different computers on my
.mac iDisk account, when on a windows computer Apple has a utility to mount
the file system, but when using Linux (Ubuntu in my case) your out of luck.

But luckily iDisk is just a webdav share so mounting it is pretty easy.

Firstly do a

> `sudo apt-get install davfs2`

This will install the required utility to mount webdav file systems.

Then fire up your favorite editor and edit

> `/etc/davfs2/secrets`

And ad a entry like this

> `http://idisk.mac.com/username USERNAME PASSWORD`

to mount the file system manually type

> `mount -t davfs http://idisk.mac.com/username /mnt/idisk`

That's it, your ready to go.

If you like to have it automatically mounted when booting you have to edit
**_/etc/fstab_** and add

> `http://idisk.mac.com/username /mnt/idisk davfs user 0 0`

