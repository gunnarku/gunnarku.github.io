
# Memory

## macOS and iOS

* [A look at how malloc works on the Mac](https://www.cocoawithlove.com/2010/05/look-at-how-malloc-works-on-mac.html) by Matt Gallagher.
* [OSX Heap Exploitation](https://blog.shpik.kr/osx,/macos,/heap,/pwnable/2019/05/09/OSX_Heap_Exploitation.html)
* [In the Zone: OS X Heap Exploitation](https://papers.put.as/papers/macosx/2016/Summercon-2016.pdf)
* [Identifying high-memory use with jetsam event reports](https://developer.apple.com/documentation/xcode/identifying-high-memory-use-with-jetsam-event-reports)
* [Handling low memory conditions in iOS and Mavericks](https://newosxbook.com/articles/MemoryPressure.html)
* [Enabling the Malloc Debugging Features](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/Articles/MallocDebug.html)

## FreeBSD

* [Exploring Swap on FreeBSD](https://klarasystems.com/articles/exploring-swap-on-freebsd/)
* [Preventing FreeBSD to kill PostgreSQL (aka OOM Killer prevention)](https://fluca1978.github.io/2021/04/02/OOMKillerFreeBSD.html)
* [typed_mem -- heap memory	accounting system](https://man.freebsd.org/cgi/man.cgi?query=FREE&amp;sektion=9)

## Android

* [Understanding Android memory usage (Google I/O '18)](https://www.youtube.com/watch?v=w7K0jio8afM)

## Linux

* [LinuxMM: OOM_Killer](https://linux-mm.org/OOM_Killer)
* [Overcommit in Linux kernel](https://www.kernel.org/doc/Documentation/vm/overcommit-accounting)
* [How to Configure the Linux Out-of-Memory Killer](https://www.oracle.com/technical-resources/articles/it-infrastructure/dev-oom-killer.html)
* [Improving the OOM killer](https://lwn.net/Articles/684945/)
* [Taming the OOM killer](https://lwn.net/Articles/317814/)
* [The "too small to fail" memory-allocation rule](https://lwn.net/Articles/627632/)
* [All the LWN articles about OOM killer](https://lwn.net/Kernel/Index/#OOM_killer)
* [Open-sourcing oomd, a new approach to handling OOMs](https://engineering.fb.com/2018/07/19/production-engineering/oomd/)
* [OOM handling](https://github.com/gperftools/gperftools/wiki/OOM-handling)
* [what is the purpose of memory overcommitment on Linux?](https://unix.stackexchange.com/questions/441364/what-is-the-purpose-of-memory-overcommitment-on-linux)

### Nuances of LD_PRELOAD and wrapping malloc() and friends

* [failmalloc](https://www.nongnu.org/failmalloc/)
* [Correct usage of LD_PRELOAD for hooking libc functions](https://tbrindus.ca/correct-ld-preload-hooking-libc/)
* [Code Injection on Linux and macOS with LD_PRELOAD](https://www.getambassador.io/blog/code-injection-on-linux-and-macos)
* [Create a wrapper function for malloc and free in C](https://stackoverflow.com/questions/262439/create-a-wrapper-function-for-malloc-and-free-in-c)
* [Malloc Hooks in Android](https://android.googlesource.com/platform/bionic/+/master/libc/malloc_hooks/README.md)
* [Securing malloc in glibc: Why malloc hooks had to go](https://developers.redhat.com/articles/2021/08/25/securing-malloc-glibc-why-malloc-hooks-had-go)
* [Replacing malloc](https://www.gnu.org/software/libc/manual/html_node/Replacing-malloc.html#Replacing-malloc)


### malloc() and NULL

Take the following with a grain of salt.

* [Four reasons to check what the malloc function returned](https://pvs-studio.com/en/blog/posts/cpp/0938/). The follow-up [discussion](https://habr.com/en/companies/pvs-studio/articles/348098/comments/#comment_10649678) in Russian.

### TLS is not easy

* [A Deep dive into (implicit) Thread Local Storage](https://chao-tic.github.io/blog/2018/12/25/tls)
* [ELF Handling For Thread-Local Storage](https://uclibc.org/docs/tls.pdf) by Ulrich Drepper.
* [Use Cases for Thread-Local Storage](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4324.html) by Paul E. McKenney.
* Bug: [Access to __thread variable may call malloc](https://sourceware.org/bugzilla/show_bug.cgi?id=16133)
* Bug: [alloc-tls: Handle thread-local storage on platforms without #[thread_local]](https://github.com/ezrosent/allocators-rs/issues/54)

## General

* [Memory Management Reference](https://www.memorymanagement.org/)
* [A Memory Allocator](https://gee.cs.oswego.edu/dl/html/malloc.html) by Doug Lea.
* [Page Size](https://www.omscs-notes.com/operating-systems/memory-management/#page-size)
* [/Zc:throwingNew (Assume operator new throws)](https://learn.microsoft.com/en-us/cpp/build/reference/zc-throwingnew-assume-operator-new-throws?view=msvc-170)

## Performance

* [Profiling Custom Memory Allocators](https://mmore500.com/2020/07/02/malloc-profile.html)
* [.NET memory analysis and diagnostics](https://github.com/Maoni0/mem-doc) by Maoni Stephens.
* [Work related to optimizing memory allocations in Firefox](https://blog.mozilla.org/nnethercote/category/memory-allocation/)
* [Tracing with GCC](https://fekir.info/post/tracing-with-gcc/)
* [Linux RCU](http://lastweek.io/notes/linux/linux-rcu/)
* [How Memory Allocation Affects Performance in Multithreaded Programs](https://www.oracle.com/technical-resources/articles/it-infrastructure/dev-mem-alloc.html)
* [Magazines and Vmem: Extending the Slab Allocator to Many CPUs and Arbitrary Resources](https://www.usenix.org/conference/2001-usenix-annual-technical-conference/magazines-and-vmem-extending-slab-allocator-many)
* [Beyond malloc efficiency to fleet efficiency: a hugepage-aware memory allocator](https://www.usenix.org/conference/osdi21/presentation/hunter)

## CppCon (and other) talks

* [How to Write a Heap Memory Profiler - Milian Wolff - CppCon 2019](https://www.youtube.com/watch?v=YB0QoWI-g8E)
* [Small is beautiful: Techniques to minimise memory footprint - Steven Pigeon - CppCon 2019)](https://www.youtube.com/watch?v=Dxy66x6v4HE)
* [Understanding Allocator Impact on Runtime Performance in C++ - Parsa Amini - CppCon 2022](https://www.youtube.com/watch?v=Ctfbs6UVJ9Y)
* [Trading at light speed: designing low latency systems in C++ - David Gross - Meeting C++ 2022](https://www.youtube.com/watch?v=8uAW5FQtcvE)
* [CppCon 2014: Paul E. McKenney "C++ Memory Model Meets High-Update-Rate Data Structures"](https://www.youtube.com/watch?v=1Q-RH2tiyt0)
* [What Programmers Should Know About Memory Allocation - S. Al Bahra, H. Sowa, P. Khuong - CppCon 2019](https://www.youtube.com/watch?v=gYfd25Bdmws)
* [Abusing Your Memory Model for Fun and Profit - Samy Al Bahra, Paul Khuong - CppCon 2019](https://www.youtube.com/watch?v=N07tM7xWF1U)
* [Building a Lock-free Multi-producer, Multi-consumer Queue for Tcmalloc - Matt Kulukundis - CppCon 21](https://www.youtube.com/watch?v=_qaKkHuHYE0)

# Allocators

* [libumem](https://en.wikipedia.org/wiki/Libumem) and its [port](https://github.com/omniti-labs/portableumem/).
