---
layout: post
title: "Ubuntu Server 6.06"
category:
tags: []
---
{% include JB/setup %}
I installed Ubuntu server on one of my machines, one of the nice things about it, is that it from install it configures a working LAMP (Linux, Apache, MySQL and PHP) set up. Which is nice and saves lots of configuration. Unfortunately, I still need to get Subversion, Ruby, Tomcat, and other things installed and running on the system. Anyways since, I was going to have to set up a bunch of things and planned on using the system as a development machine I then installed Ubuntu desktop on the system as one of the aptitude scripts, which installs all the packages require for the desktop configuration. After that though, I realized that I was not able to complete any install with out causing an error in clvm, anything you install would cause a clvm error and make your install fail. So here is the fix if you install the Ubuntu server from CD and then install the desktop:

Ultimately this post by npcomplete2000, was the solution for me:
<a href="http://www.ubuntuforums.org/archive/index.php/t-186356.html">http://www.ubuntuforums.org/archive/index.php/t-186356.html</a>

removing clvm caused no problems for me and was something I never thought I would need. After that I could install other applications with out problems.

<b>More error information so those searching for error codes will find this post:</b>
Starting Cluster LVM Daemon clvmd could not connect to cluster manager
Consult syslog for more information
invoke-rc.d: initscript clvm, action "start" failed.
dpkg: error processing clvm (--configure):
 subprocess post-installation script returned error exit status 3
Errors were encountered while processing:
 clvm
E: Sub-process /usr/bin/dpkg returned an error code (1)