
# Software development

## iOS and OS X

* [*OS Internals Book](https://www.newosxbook.com/home.html)
* [Linking Objective-C Code](https://pewpewthespells.com/blog/objc_linker_flags.html)
* [GCD Internals](https://newosxbook.com/articles/GCD.html) by Jonathan Levin.
* [Synchronization Primitives - Kernel Programming Guide](https://developer.apple.com/library/archive/documentation/Darwin/Conceptual/KernelProgramming/synchronization/synchronization.html#//apple_ref/doc/uid/TP30000905-CH218-BEHJDFCA)
* [Threading Programming Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/Multithreading/CreatingThreads/CreatingThreads.html#//apple_ref/doc/uid/10000057i-CH15-SW7)
* [Dispatch Queues - Concurrency Programming Guide](https://developer.apple.com/library/archive/documentation/General/Conceptual/ConcurrencyProgrammingGuide/OperationQueues/OperationQueues.html#//apple_ref/doc/uid/TP40008091-CH102-SW1)
* [Dancing in the Debugger — A Waltz with LLDB](https://www.objc.io/issues/19-debugging/lldb-debugging/) by Ari Grant.
* [NSAssertionHandler](https://nshipster.com/nsassertionhandler/) by Mattt.
* [Method Swizzling](https://nshipster.com/method-swizzling/) by Mattt.
* [Building Efficient OS X Apps - Session 704](https://asciiwwdc.com/2013/sessions/704). The WWDC archive is [here](https://pvieito.com/2022/05/wwdc-sessions-archive).
* [Building Responsive and Efficient Apps with GCD - Session 718](https://asciiwwdc.com/2015/sessions/718)
* [Synchronization - Threading Programming Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/Multithreading/ThreadSafety/ThreadSafety.html#//apple_ref/doc/uid/10000057i-CH8-SW14)
* [iOS Debugging Magic - Technical Note TN2239](https://developer.apple.com/library/archive/technotes/tn2239/_index.html#//apple_ref/doc/uid/DTS40010638-CH1-SUBSECTION19)
* [Thread Safe vs Thread Un-Safe](https://izeeshan.wordpress.com/tag/nsthread/)
* [Building Objective-C static libraries with categories](https://developer.apple.com/library/archive/qa/qa1490/_index.html)
* [Reducing iOS app size using linker and why_load](https://asifmohd.github.io/ios/2023/03/30/reducing-ios-app-size-using-linker.html)
* [Two years of issues on advanced iOS and macOS development](https://www.objc.io/issues/#19)
* [RE:Trace – Applied Reverse Engineering on OS X](https://www.defcon.org/images/defcon-16/dc16-presentations/defcon-16-beauchamp-weston.pdf)
* [Source for objc-initialize.mm](https://opensource.apple.com/source/objc4/objc4-723/runtime/objc-initialize.mm.auto.html)

### Basic

* [MacOS Developer Setup](https://www.chrisatmachine.com/posts/01-macos-developer-setup)
* [Moving to zsh – MacSysAdmin 2019](https://scriptingosx.com/zsh/)
* [The Biggest & Best List of Mac Keystrokes](https://www.danrodney.com/mac/)
* [Instruments Help](https://help.apple.com/instruments/mac/current/)
* [How to debug an iOS app with lldb on the command line on a device without Xcode](https://stackoverflow.com/questions/26934393/how-to-debug-an-ios-app-with-lldb-on-the-command-line-on-a-device-without-xcode)
* [NSObject +load and +initialize - What do they do?](https://stackoverflow.com/questions/13326435/nsobject-load-and-initialize-what-do-they-do)

## Debugging

### GDB

* [Beej's Quick Guide to GDB](http://beej.us/guide/bggdb/)
* [LLDB to GDB Command Map](http://lldb.llvm.org/lldb-gdb.html)
* [GDB Vs. WinDbg Commands | Technokrafti's Weblog](https://blogsai.wordpress.com/2009/11/30/gdb-and-windbg/)
* [How can I scroll back in GDB's command window in the TUI mode? - Stack Overflow](http://stackoverflow.com/questions/9257085/how-can-i-scroll-back-in-gdbs-command-window-in-the-tui-mode)


## tmux

* [tmux shortcuts & cheatsheet](tmux shortcuts & cheatsheet)
* [Making tmux Pretty and Usable - A Guide to Customizing your tmux.conf](http://www.hamvocke.com/blog/a-guide-to-customizing-your-tmux-conf/)
* [Self-contained, pretty and versatile .tmux.conf configuration file](https://github.com/gpakosz/.tmux)
* [How to copy to system clipboard from tmux output after mouse selection?](https://stackoverflow.com/questions/12287432/how-to-copy-to-system-clipboard-from-tmux-output-after-mouse-selection)

## All things BSD

* [A curated list of awesome OpenBSD resources](https://github.com/ligurio/awesome-openbsd)
* [The FreeBSD Desktop series](https://vermaden.wordpress.com/freebsd-desktop/)
* [Challenge accepted: OpenBSD on a laptop](https://jpmens.net/2019/04/06/challenge-accepted-openbsd-on-a-laptop/)
* [OpenBSD on a Laptop](https://www.c0ffee.net/blog/openbsd-on-a-laptop)
* [OpenBSD on the Lenovo ThinkPad X1 Carbon (5th Gen)](https://jcs.org/2017/09/01/thinkpad_x1c)
* [Prepare ThinkPad X1 Carbon Gen 5 for OpenBSD](https://romanzolotarev.com/openbsd/lenovo-thinkpad-x1c5.html)
* [OpenBSD on the Desktop (Part I)](https://www.paedubucher.ch/articles/open-bsd-on-the-desktop-part-1/) and [Part II](https://www.paedubucher.ch/articles/open-bsd-on-the-desktop-part-2/)
* [Building only kernel by new build infrastructure OpenBSD-current](https://daemonforums.org/showthread.php?t=10020)
* [Small is Beautiful and Other Thoughts on Programming Strategies - BSDCon 2002 Paper](https://www.usenix.org/legacy/publications/library/proceedings/bsdcon02/mashey_small/)

## Linux

* [Linux x86 Program Start Up or - How the heck do we get to main()?](http://dbp-consulting.com/tutorials/debugging/linuxProgramStartup.html)
* [Replacing x86 firmware with Linux and Go](https://lwn.net/Articles/738649/)
* [How to use the Linux AIO feature](https://github.com/littledan/linux-aio)
* [What is the status of POSIX asynchronous I/O (AIO)?](https://stackoverflow.com/questions/87892/what-is-the-status-of-posix-asynchronous-i-o-aio/5307557#5307557)
* [Linux AIO Performance and Robustness for Enterprise Workloads](https://www.kernel.org/doc/ols/2004/ols2004v1-pages-63-78.pdf)
* [Getting started debugging on Linux](https://media.steampowered.com/apps/steamdevdays/slides/debugging.pdf)
* [Linux Performance](http://www.brendangregg.com/linuxperf.html)
* [Linux Profiling and Optimization The Black Art of Linux Performance Tuning](https://www.cs.princeton.edu/picasso/mats/mats_S07/Lucifredi_Lecture_Feb07.pdf)

## Random

* [Game Theory and Probability for Bitcoin](https://github.com/micah541/GameTheory)
