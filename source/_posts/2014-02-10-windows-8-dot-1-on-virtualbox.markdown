---
layout: post
title: "Windows 8.1 on VirtualBox"
date: 2014-02-10 14:11:32 -0600
comments: true
categories: [Geekery,IT]
---
[idvirtualbox]: http://virtualbox.org
Running multiple environments is critical for me both in IT and web development. I'm currently using [virtualbox][idvirtualbox] on my Mac to virtualize a windows 8.1 environment (I know, I know...). Click through for a quick walkthrough.
<br>
![Win 8.1 VM](/images/win8vm/win8vm4.png)
<br>
<!--more-->
I'm using virtualbox over more popular alternatives such as VMWare Fusion and Parallels because of it's opensource nature and more technical community background. Windows 8.1 takes a little bit more time to configure, but it installs the same as any other VM.
<br>
![win 8.1 vm settings](/images/win8vm/win8vm.png)
<br>
1. Create a new VM shell, be sure to select your correct distro and x86 vs x64
2. Boot to your ISO, PXE, disk, etc
3. Install like normal
4. Attempt to boot

If you're having difficulties booting, check your storage controller and chipset config. I had trouble creating a SATA controller and booting to network (PXE boot), so I had to use an IDE virtual disk.
<br>
![controller settings](/images/win8vm/win8vm2.png)
<br>
Assign RAM and cpu appropriately, and select ICH9 chipset if you have issues.
<br>
![chipset settings](/images/win8vm/win8vm3.png)
<br>
