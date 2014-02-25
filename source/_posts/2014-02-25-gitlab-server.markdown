---
layout: post
title: "GitLab Server"
date: 2014-02-25 12:19:21 -0600
comments: true
categories: [IT,Web]
---
<br>
[gitlaburl]: http://www.gitlab.com/
Recently I had the opportunity to install, configure, and work off of a new [Gitlab][gitlaburl] installation in our office. We're slowly building a design and development team, and needed a solution for code versioning and project management.
<br>
![GitLab](/images/gitlab/gitlab.png)
<br>
<!--more-->
[gitlabinstallurl]: http://gitlab.com/gitlab-org/gitlab-ci/blob/master/doc/install/installation.md
Installation took roughly 2 hours, and Gitlab provides a very detailed walkthrough [here][gitlabinstallurl] for Ubuntu and Deb. I'm running this on a Ubuntu 12.04 VM locally in our office, and haven't had any real issues with it besides some complications with email flow. When running email through an exchange server like we are at the office, some extra tweaks are needed to the config files and exch server.

Once Gitlab is installed and your SSH keys are set up properly, it functions nearly exactly like github does. Creating projects, cloning repos, and creating user accounts is a breeze.
<br>
![Gitlab New Project](/images/gitlab/gitlab2.png)
<br>
Having trouble in Gitlab? Be sure to check the logs tabs to see what's going on.
<br>
![Gitlab Logs](/images/gitlab/gitlab3.png)
<br>
