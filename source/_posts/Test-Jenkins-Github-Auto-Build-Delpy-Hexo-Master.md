---
title: Test Jenkins Github Auto Build Delpy Hexo Master
date: 2017-12-14 23:28:23
tags: hexo,Jenkins,github
---

### What does the fox say?

#### ding ~~.~~ ding ~~.~~ ding

`public static void main(String[] args){System.out.println("Hello Hexo , Hello Github")}`


### Jenkins Console Log
```Javascript
Started by GitHub push by jianbinhusky
Building in workspace /var/lib/jenkins/workspace/blog
 > /usr/bin/git rev-parse --is-inside-work-tree # timeout=10
Fetching changes from the remote Git repository
 > /usr/bin/git config remote.origin.url https://github.com/jianbinhusky/jianbinhusky.github.io.git # timeout=10
Fetching upstream changes from https://github.com/jianbinhusky/jianbinhusky.github.io.git
 > /usr/bin/git --version # timeout=10
using GIT_ASKPASS to set credentials
 > /usr/bin/git fetch --tags --progress https://github.com/jianbinhusky/jianbinhusky.github.io.git +refs/heads/*:refs/remotes/origin/*
 > /usr/bin/git rev-parse refs/remotes/origin/develop^{commit} # timeout=10
 > /usr/bin/git rev-parse refs/remotes/origin/origin/develop^{commit} # timeout=10
Checking out Revision 7979756216fbef607e3b2c699e7ede19aed23f4d (refs/remotes/origin/develop)
 > /usr/bin/git config core.sparsecheckout # timeout=10
 > /usr/bin/git checkout -f 7979756216fbef607e3b2c699e7ede19aed23f4d
Commit message: "write something to re-test shell script for jenkins and github auto deploy"
 > /usr/bin/git rev-list 0a36a7eeabaafdafff63a269bb2b35b3f7fe9d7c # timeout=10
[blog] $ /bin/sh -xe /tmp/jenkins7625280691553334127.sh
+ BUILD_ID=dontKillMe /home/blog.sh
++++++++++++++++++++++++++++++++
cd ---> /var/lib/jenkins/workspace/blog
[sudo] jenkins 的密码： npm WARN optional SKIPPING OPTIONAL DEPENDENCY: fsevents@1.1.3 (node_modules/fsevents):
npm WARN notsup SKIPPING OPTIONAL DEPENDENCY: Unsupported platform for fsevents@1.1.3: wanted {"os":"darwin","arch":"any"} (current: {"os":"linux","arch":"x64"})

added 116 packages in 4.443s
INFO  Deleted database.
INFO  Deleted public folder.
INFO  Start processing
INFO  Files loaded in 285 ms
INFO  Generated: index.html
INFO  Generated: archives/index.html
INFO  Generated: fonts/default-skin.b257fa.svg
INFO  Generated: img/default-skin.png
INFO  Generated: main.0cf68a.css
INFO  Generated: slider.e37972.js
INFO  Generated: main.0cf68a.js
INFO  Generated: mobile.992cbe.js
INFO  Generated: fonts/iconfont.16acc2.ttf
INFO  Generated: fonts/iconfont.45d7ee.svg
INFO  Generated: fonts/iconfont.8c627f.woff
INFO  Generated: fonts/iconfont.b322fa.eot
INFO  Generated: fonts/tooltip.4004ff.svg
INFO  Generated: img/preloader.gif
INFO  Generated: img/scrollbar_arrow.png
INFO  Generated: archives/2017/12/index.html
INFO  Generated: tags/hexo-Jenkins-github/index.html
INFO  Generated: archives/2017/index.html
INFO  Generated: 2017/12/14/Test-Jenkins-Github-Auto-Build-Delpy-Hexo-Master/index.html
INFO  Generated: 2017/12/14/hello-world/index.html
INFO  20 files generated in 149 ms
FATAL Something's wrong. Maybe you can find the solution here: http://hexo.io/docs/troubleshooting.html
Error: EACCES: permission denied, open '/var/lib/jenkins/workspace/blog/db.json'
FATAL EACCES: permission denied, open '/var/lib/jenkins/workspace/blog/db.json'
Error: EACCES: permission denied, open '/var/lib/jenkins/workspace/blog/db.json'
deploy done!
Go to github to double-confirm -------> https://github.com/jianbinhusky/jianbinhusky.github.io
Go to my blog -----> https://jianbinhusky.github.io
++++++++++++++++++++++++++++++++
Finished: SUCCESS
```
