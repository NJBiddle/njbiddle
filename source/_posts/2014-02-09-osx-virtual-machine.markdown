---
layout: post
title: "OSX Virtual Machine"
date: 2014-02-09 19:03:17 -0600
comments: true
categories: [Geekery,IT]
---
Using a spare machine, I've successfully set up a headless OSX VM on intel-based hardware. It's relatively under-powered, but serves my needs as a small file server and iTunes box.
<br>
![OSX VM](/images/osxvm/osxvm4.png)
<br>
<!--more-->
[esxi]: http://vmwarelearning.com/esxi/
[donk]: http://www.insanelymac.com/forum/topic/267296-esxi-5-mac-os-x-unlocker/
This was accomplished by running [ESXi5.1][esxi] patched with [Donk's OSX unlocker][donk]. After patching, you'll need to upload the OSX installation .dmg and boot to ISO.
<br>
![OSX VM2](/images/osxvm/osxvm2.png)
<br>
Install OSX to your assigned datastore and your VM should boot right up. Originally I did this install with osx 10.8, but have since updated to 10.9 Mavericks. For the upgrade:

1. Snapshot the VM
2. Run the upgrade as normal
3. Reboot when prompted
4. Success!
5. Remove that snapshot

Assign USB devices, more ram, cores, etc for added functionality and performance.
<br>
![OSX VM3](/images/osxvm/osxvm3.png)
<br>
