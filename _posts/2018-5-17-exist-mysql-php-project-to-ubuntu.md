---
layout: post
title: Copying Mysql PHP Project to Ubuntu
date: 2018-5-17
---
Press Ctrl+Alt+T to release Terminal.  
type sudo nautilus

Then a window will be open.  
Go to File System > var > www  
Paste your folder project there.

If you access via localhost it would say Forbidden.

To make it accessible you need to change Properties
of the folder and it files inside.

For the folder permission the Folder access will be  
Access files  
Access files

For each file permission the Access will be  
Read-only  
Read-only

Then it can be access via localhost.
Otherwise, the mistaken on the CMS the system itself.

For example, if there are .htaccess make sure
the file there and can be used.

In my case the .htaccess created later on Windows,
the file has not shown on Ubuntu. But on Windows
still exist.
