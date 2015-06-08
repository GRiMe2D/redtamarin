| **note:** merge this FAQ with the web site FAQ, re-edit for CLIB, RNL and AVMGlue |
|:----------------------------------------------------------------------------------|


---


  * **What's the main difference with [Tamarin](http://www.mozilla.org/projects/tamarin/) ?**
> Tamarin focus on VM and optimization (like GC, nanoJIT, etc.), redtamarin focus on shell and APIs.

  * **Why use SVN when Tamarin use [Mercurial](http://www.selenic.com/mercurial/) ?**
> Mainly because I prefer SVN (yep arbitrary choice) and also because [gclient](http://code.google.com/p/maashaack/wiki/gclient) does not support mercurial.

  * **Which Operating System are supported ?**
> Most of the ones that Tamarin supports, mainly OS X, Windows and Linux (Ubuntu),
> but others as Android, Windows CE, Solaris, etc. could also be supported (testers welcome).

  * **Why not Java or .NET ?**
> Because they do not work with the Tamarin VM and do not support the AS3 language.

  * **Why the focus on command-line tools with ActionScript 3 ?**
> Because it's missing in the regular AS3 toolchain and command-line tools can save your butt
> on numerous occasions.

  * **What are `*.abc` files ?**
> [Actionscript ByteCode](ABC.md) files generated by the [ActionScript Compiler](ASC.md).

  * **How an executable is generated from `*.abc` ?**
> ASC have options that allow you to produce an `*.exe` that basically embed an `*.abc` file, see the documentation for [projectors](Projector.md).

  * **Does the executable have dependencies ?**
> Nope. You obtain a single independant executable.

  * **Are they similar tools out there ?**
> Yes, look at [JSDB](http://www.jsdb.org/), it's the same principle, it's the [SpiderMonkey engine](http://www.mozilla.org/js/spidermonkey/) running on the command-line that can embed JavaScript files in a single executable.

  * **What's the use of the C libraries (stdlib, etc.) under AS3 ?**
> On one part, it promotes the porting of C source code to AS3 source code, that way some AS3 coder can extends those command-line tools more easyly with their language of choice (AS3), and on another part, it promotes C coders to get interested at the AS3 language without missing C functions they are used to.

  * **What's the use of the flash platform APIs ?**
> It allows to port existing AS3 source code, targeted at the [Flash player](http://www.adobe.com/products/flashplayer/) or [AIR](http://www.adobe.com/products/air/), to work on the command-line.
