---
author: connylundgren
date: '2007-07-05 09:50:48'
layout: post
slug: boosting-you-productivity-in-eclipse-using-shortcuts
status: publish
title: Boosting you productivity in Eclipse using shortcuts
wordpress_id: '105'
categories:
- ide, eclipse
comments: true
---

Recently a team member approached me wanting to switch IDE from the corporate
standard Borland JBuilder to Eclipse, and she asked if I had some nice advice
to boost productivity. Well using keyboard shortcuts is IMHO a huge
productivity booster, and I compiled a list of my 13 most used shortcuts I
find useful in my everyday work.

The hard part about shortcuts is that I never seem to be able to say which
combination to press, they are just subconscious. Start saving some time,
learn them, perhaps not all but everyone of them will save you quite some time
over a day of use.

**Note**: _If your using OS X exchange CTRL with the Command key_

So buckle up, and start being more productive right now..

  

### Open type** (ctrl + shift + T)**

This will open up a class in the workspace (or in dependencies such as jar-
files), the dialog accepts wildcards (for instance ***Action**), another nifty
feature are the _CamelCase _notation to quickly open a file, for instance if
you want to open the class **HotelBookingAction **entering **HBA**´would give
you the correct result right away, and save you some typing.

![](http://blog.refactor.se/static/images/105/open_type.png)

  

### Open Resource** (ctrl + shift + R)**

Same tip as above, but it works on every resource (.jsp, .properties, .xml
etc) in your workspace, same tips for wildcards as above applies.

![](http://blog.refactor.se/static/images/105/open_resource.png)

  

### Navigate to member **(ctrl + O)**

You know, even if you probably shouldn't you have some class which is really
large, several hundreds of code, maybe even thousands. How do you navigate to
a member (method, variable) one option (and most often used) is to search for
it using Ctrl + F, it's really not that efficient, instead use this short cut
to list all the methods, to narrow the list start typing the method name
navigate to the one you want with the arrow keys and press enter. Even more,
press the key another time and it will show you the inherited members.

![](http://blog.refactor.se/static/images/105/navigate_to_member.png)

  

### Go to Line** (ctrl + L)**

Often you find a line number when digging through stack traces and such, to
simply go to a line in the open file press Cmd + L and enter the line number.

![](http://blog.refactor.se/static/images/105/go_to_line.png)

  

### Go to last edit** (ctrl +Q)**

Do you know the scenario when you edit your large class file, and you change
something in one method, and want to go to the last thing you edited in before
this? Instead of browsing to the previous method, finding the right spot use
this command to jump right back to the last edit, use it multiple times to
track back in history.

  

### Show type hirarchy** (ctrl + T)**

This one took me quite some time to find, usually i just jump to the top of
the class, find the supertype and hit F3 to open the supertype, with this the
power are at your fingertips.

![](http://blog.refactor.se/static/images/105/show_type_hirarchy.png)

  

### Go to open editor** (ctrl + E)**

I often keep some 10 editor windows open at any given time (or more), if you
want an easy way to switch between open editors try this command, either
select the file you want to bring to the front, or start typing to narrow the
results down a bit.

![](http://blog.refactor.se/static/images/105/go_to_open_editor.png)

  

### Next error/warning** (ctrl + +.**

This command will cycle through the errors/warnings in the current file,
instead of using the Problems view. I tend not to use this so often, the this
since the short not that intuitive (easily fixed by remapping, but then I
would go nuts when using another machine).

  

### Move block of code** (alt + arrow up/down)**

Often find yourself copying and pasting code while moving around declarations,
or whole block of code? No more, this shortcut will move a line (or block) of
code up/down one line much easier and faster than cut’n’paste.

  

### Block comment/uncomment** (Shift + Ctrl + /)**

Instead of commenting out blocks of code with /* */ use this, it will make
every selected line commented out with a // , to remove the comment invoke
this again to remove.

  

### Search workspace for references** (ctrl + shift + G)**

Do you want to know if anyone is calling your method, or using the variable?
Find the method, invoke this command and se the results of all references in
the workspace.

  

### Reformat code** (ctrl + shift + F)**

Apply the current code formatting set to the open file, this one is pretty
much etched in mine spine doing this just before I commit/save a class.

  

### Organize imports** (ctrl + Shift + O)**

Do you want to keep you imports nice and tidy, and organized according to the
preferences?

