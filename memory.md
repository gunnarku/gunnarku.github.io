
# Memory

## macOS and iOS

* [A look at how malloc works on the Mac](https://www.cocoawithlove.com/2010/05/look-at-how-malloc-works-on-mac.html) by Matt Gallagher.
* [OSX Heap Exploitation](https://blog.shpik.kr/osx,/macos,/heap,/pwnable/2019/05/09/OSX_Heap_Exploitation.html)
* [In the Zone: OS X Heap Exploitation](https://papers.put.as/papers/macosx/2016/Summercon-2016.pdf)
* [Identifying high-memory use with jetsam event reports](https://developer.apple.com/documentation/xcode/identifying-high-memory-use-with-jetsam-event-reports)
* [Handling low memory conditions in iOS and Mavericks](https://newosxbook.com/articles/MemoryPressure.html)
* [Enabling the Malloc Debugging Features](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/Articles/MallocDebug.html)
* [iOS WeChat memory monitoring](https://www.programmersought.com/article/7089701673/)
* [VM Tracker for iOS memory in-depth exploration](https://www.programmersought.com/article/2794632201/)
* [iOS Debugging Magic](https://developer.apple.com/library/archive/technotes/tn2239/_index.html)
* [Using Dynamic Libraries](https://developer.apple.com/library/archive/documentation/DeveloperTools/Conceptual/DynamicLibraries/100-Articles/UsingDynamicLibraries.html)
* [Trace Dynamic Memory Allocations](https://craftware.xyz/tips/Trace-memory-allocations.html)
* [Page Cache, the Affair Between Memory and Files](https://manybutfinite.com/post/page-cache-the-affair-between-memory-and-files/)
* [About Memory Management | Advanced Memory Management Programming Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/MemoryMgmt/Articles/MemoryMgmt.html#//apple_ref/doc/uid/10000011i)
* [About the Virtual Memory System | Memory Usage Performance Guidelines](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/Articles/AboutMemory.html). Start from the [top](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/ManagingMemory.html#//apple_ref/doc/uid/10000160i). Definitely read [Tips for Allocating Memory](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/Articles/MemoryAlloc.html).
* [iOS Memory Deep Dive](https://developer.apple.com/videos/play/wwdc2018/416/)
* [No pressure, Mon! Handling low memory conditions in iOS and Mavericks](https://newosxbook.com/articles/MemoryPressure.html)

## FreeBSD

* [Exploring Swap on FreeBSD](https://klarasystems.com/articles/exploring-swap-on-freebsd/)
* [Preventing FreeBSD to kill PostgreSQL (aka OOM Killer prevention)](https://fluca1978.github.io/2021/04/02/OOMKillerFreeBSD.html)
* [typed_mem -- heap memory	accounting system](https://man.freebsd.org/cgi/man.cgi?query=FREE&amp;sektion=9)

## Android

* [Understanding Android memory usage (Google I/O '18)](https://www.youtube.com/watch?v=w7K0jio8afM)
* [Debugging Native Memory Use](https://source.android.com/docs/core/tests/debug/native-memory)
* [Is this explanation about VSS/RSS/PSS/USS accurate?](https://stackoverflow.com/questions/22372960/is-this-explanation-about-vss-rss-pss-uss-accurate)

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
* [Kernel Korner - Allocating Memory in the Kernel](https://www.linuxjournal.com/article/6930)

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
* Bug: [alloc-tls: Handle thread-local storage on platforms without thread_local](https://github.com/ezrosent/allocators-rs/issues/54)

## General

* [Memory Management Reference](https://www.memorymanagement.org/)
* [A Memory Allocator](https://gee.cs.oswego.edu/dl/html/malloc.html) by Doug Lea.
* [Page Size](https://www.omscs-notes.com/operating-systems/memory-management/#page-size)
* [/Zc:throwingNew (Assume operator new throws)](https://learn.microsoft.com/en-us/cpp/build/reference/zc-throwingnew-assume-operator-new-throws?view=msvc-170)
* [All papers written by PDOS (MIT Parallel & Distributed Operating Systems Group) since '93](https://pdos.csail.mit.edu/publications/)
* [Malloc Internals and You](https://developers.redhat.com/blog/2017/03/02/malloc-internals-and-you) by DJ Delorie.
* [A look at how malloc works on the Mac](https://www.cocoawithlove.com/2010/05/look-at-how-malloc-works-on-mac.html) by Matt Gallagher.
* [Heap: Pleasures and Pains](https://learn.microsoft.com/en-us/previous-versions/ms810466(v=msdn.10)) by Murali R. Krishnan.
* [Some things I've learned about memory](https://neugierig.org/software/blog/2011/05/memory.html)
* [Persistent Memory Allocation](https://queue.acm.org/detail.cfm?id=3534855&doi=10.1145%2F3534855)
* [How to exploit a double free vulnerability in 2021](https://github.com/stong/how-to-exploit-a-double-free)

## Performance

* [Random ASCII – tech blog of Bruce Dawson](https://randomascii.wordpress.com/)
* [Understand the Impact of Low-Lock Techniques in Multithreaded Apps](https://learn.microsoft.com/en-us/archive/msdn-magazine/2005/october/understanding-low-lock-techniques-in-multithreaded-apps) by Vance Morrison.
* [Concurrency: What Every Dev Must Know About Multithreaded Apps](https://learn.microsoft.com/en-us/archive/msdn-magazine/2005/august/concurrency-what-every-dev-must-know-about-multithreaded-apps) by Vance Morrison.
* [Profiling Custom Memory Allocators](https://mmore500.com/2020/07/02/malloc-profile.html)
* [.NET memory analysis and diagnostics](https://github.com/Maoni0/mem-doc) by Maoni Stephens.
* [Work related to optimizing memory allocations in Firefox](https://blog.mozilla.org/nnethercote/category/memory-allocation/)
* [Tracing with GCC](https://fekir.info/post/tracing-with-gcc/)
* [Linux RCU](http://lastweek.io/notes/linux/linux-rcu/)
* [How Memory Allocation Affects Performance in Multithreaded Programs](https://www.oracle.com/technical-resources/articles/it-infrastructure/dev-mem-alloc.html)
* [Magazines and Vmem: Extending the Slab Allocator to Many CPUs and Arbitrary Resources](https://www.usenix.org/conference/2001-usenix-annual-technical-conference/magazines-and-vmem-extending-slab-allocator-many)
* [Beyond malloc efficiency to fleet efficiency: a hugepage-aware memory allocator](https://www.usenix.org/conference/osdi21/presentation/hunter)
* [TfMallocTag Class Reference](https://openusd.org/docs/api/class_tf_malloc_tag.html)
* [You Can Do Any Kind of Atomic Read-Modify-Write Operation](https://preshing.com/20150402/you-can-do-any-kind-of-atomic-read-modify-write-operation/)
* [Concurrency in  C++11](https://people.cs.pitt.edu/~xianeizhang/notes/Concurrency.html)
* [Pool tag quick scanning for windows memory analysis](https://www.sciencedirect.com/science/article/pii/S1742287616000062)
* [Concurrency Freaks](https://concurrencyfreaks.blogspot.com/)
* [Is passing arguments as const references premature optimization?](https://softwareengineering.stackexchange.com/questions/372105/is-passing-arguments-as-const-references-premature-optimization)
* [Tuning Oracle databases](https://tanelpoder.com/)
* [Chrome OS Out of Memory Design](https://www.chromium.org/chromium-os/chromiumos-design-docs/out-of-memory-handling/)
* [Examining Problematic Memory in C/C++ Applications with BPF, perf, and Memcheck](https://doordash.engineering/2021/04/01/examining-problematic-memory-with-bpf-perf-and-memcheck/)
* [Clownshoes available in sizes 2^10+1 and up!](https://blog.mozilla.org/nnethercote/2011/08/05/clownshoes-available-in-sizes-2101-and-up/)
* [Beyond malloc efficiency to fleet efficiency](https://cloud.google.com/blog/topics/systems/trading-off-malloc-costs-and-fleet-efficiency)

## CppCon (and other) talks

* [How to Write a Heap Memory Profiler - Milian Wolff - CppCon 2019](https://www.youtube.com/watch?v=YB0QoWI-g8E)
* [Small is beautiful: Techniques to minimise memory footprint - Steven Pigeon - CppCon 2019)](https://www.youtube.com/watch?v=Dxy66x6v4HE)
* [Understanding Allocator Impact on Runtime Performance in C++ - Parsa Amini - CppCon 2022](https://www.youtube.com/watch?v=Ctfbs6UVJ9Y)
* [Trading at light speed: designing low latency systems in C++ - David Gross - Meeting C++ 2022](https://www.youtube.com/watch?v=8uAW5FQtcvE)
* [CppCon 2014: Paul E. McKenney "C++ Memory Model Meets High-Update-Rate Data Structures"](https://www.youtube.com/watch?v=1Q-RH2tiyt0)
* [What Programmers Should Know About Memory Allocation - S. Al Bahra, H. Sowa, P. Khuong - CppCon 2019](https://www.youtube.com/watch?v=gYfd25Bdmws)
* [Abusing Your Memory Model for Fun and Profit - Samy Al Bahra, Paul Khuong - CppCon 2019](https://www.youtube.com/watch?v=N07tM7xWF1U)
* [Building a Lock-free Multi-producer, Multi-consumer Queue for Tcmalloc - Matt Kulukundis - CppCon 21](https://www.youtube.com/watch?v=_qaKkHuHYE0)

# Papers and references on allocators and memory management

* [A bounded memory allocator for software-defined global address spaces](https://dl.acm.org/doi/10.1145/3241624.2926709)
* [Allocators in Rust](https://github.com/ezrosent/allocators-rs)
* [libumem](https://en.wikipedia.org/wiki/Libumem) and its [port](https://github.com/omniti-labs/portableumem/).
* [CLMalloc: contiguous memory management mechanism for large-scale CPU-accelerator hybrid architectures](https://doi.org/10.1117/12.2660807)
* [CustoMalloc: efficient synthesized memory allocators](https://dl.acm.org/doi/10.1002/spe.4380230804)
* [DieHard](https://github.com/emeryberger/DieHard)
* [dlmalloc](https://gee.cs.oswego.edu/dl/html/malloc.html)
* [dnmalloc](https://fossies.org/linux/misc/samhain-4.5.0.tar.gz/samhain-4.5.0/src/dnmalloc.c)
* scalloc: [Fast, multicore-scalable, low-fragmentation memory allocation through large virtual memory and global data structures](https://dl.acm.org/doi/10.1145/2814270.2814294). Source code is [here](https://github.com/cksystemsgroup/scalloc). Project page is [here](http://scalloc.cs.uni-salzburg.at/).
* ffmalloc
* FLFUMSA
* [FreeGuard](https://github.com/UTSASRG/FreeGuard)
* [Guarder](https://github.com/UTSASRG/Guarder)
* [Hardened malloc](https://github.com/GrapheneOS/hardened_malloc/)
* HMalloc
* [Hoard](https://github.com/emeryberger/Hoard)
* [How Hard is it to Adapt a Memory Allocator to CHERI?](https://tratt.net/laurie/blog/2023/how_hard_is_it_to_adapt_a_memory_allocator_to_cheri.html)
* [Identifying Memory Allocation Patterns in HEP Software](https://cds.cern.ch/record/2298615/files/pdf.pdf). Here's how malloc interpose [is implemented](https://github.com/FOM-Tools/FOM-Tools/blob/master/src/mallocinterpose.cxx).
* [Intel TBB allocator](https://github.com/oneapi-src/oneTBB)
* [IsoAlloc](https://github.com/struct/isoalloc)
* [jemalloc](https://github.com/jemalloc)
* [jmalloc](https://github.com/Aalto5G/jmalloc)
* [kmalloc](https://github.com/freebsd/freebsd-src/blob/main/libexec/rtld-elf/rtld_malloc.c)
* LFMalloc
* LFMalloc
* LFMallocwoGC
* LKmalloc
* [Lock-free memory allocator without garbage collection on multicore embedded devices](https://ieeexplore.ieee.org/document/6776071)
* [Lockless](http://locklessinc.com/)
* LRMalloc
* [ltalloc](https://github.com/alextretyak/ltalloc)
* [Makalu: fast recoverable allocation of non-volatile memory](https://dl.acm.org/doi/10.1145/2983990.2984019). Source code is [here](https://github.com/HewlettPackard/Atlas/tree/makalu).
* MarkUs
* [Mallacc: Accelerating Memory Allocation](https://dl.acm.org/doi/10.1145/3093337.3037736)
* MCMalloc
* [McRT-Malloc: a scalable transactional memory allocator](https://dl.acm.org/doi/abs/10.1145/1133956.1133967)
* PAllocator: [Memory management techniques for large-scale persistent-main-memory systems](https://dl.acm.org/doi/abs/10.14778/3137628.3137629)
* [Mesh](https://github.com/plasma-umass/Mesh)
* [Mostly lock-free malloc](https://dl.acm.org/doi/abs/10.1145/512429.512451)
* [MPKAlloc](https://github.com/BUseclab/mpkalloc)
* mtmalloc: [article here](https://www.oracle.com/technical-resources/articles/it-infrastructure/dev-mem-alloc.html) and [manual here](https://docs.oracle.com/cd/E88353_01/html/E37843/mtmalloc-3malloc.html)
* [musl malloc](https://musl.libc.org/)
* [NBMALLOC: Allocating Memory in a Lock-Free Manner](https://link.springer.com/article/10.1007/s00453-008-9268-x). See [this paper](https://link.springer.com/chapter/10.1007/11561071_31) as well. Project page is [here](https://www.cse.chalmers.se/research/group/dcs/nbmalloc.html).
* [nedmalloc](https://github.com/ned14/nedmalloc)
* [NUMAlloc: A Faster NUMA Memory Allocator](https://dl.acm.org/doi/10.1145/3591195.3595276)
* [NVAlloc: rethinking heap metadata management in persistent memory allocators](https://dl.acm.org/doi/10.1145/3503222.3507743). Source code is [here](https://github.com/ISCS-ZJU/NVAlloc).
* [ottomalloc](https://github.com/openbsd/src/blob/master/lib/libc/stdlib/malloc.c)
* [PartitionAlloc](https://chromium.googlesource.com/chromium/src/+/main/base/allocator)
* [phkmalloc](https://github.com/emeryberger/Malloc-Implementations/tree/master/allocators/phkmalloc)
* [Profiling a warehouse-scale computer](https://dl.acm.org/doi/10.1145/2749469.2750392)
* [ptmalloc3](http://www.malloc.de/en/)
* ptlbmalloc2
* Rockall
* [rpmalloc](ttps://github.com/mjansson/rpmalloc)
* [Scalable lock-free dynamic memory allocation](https://dl.acm.org/doi/10.1145/996893.996848)
* [Scudo](https://source.android.com/docs/security/test/scudo)
* [SFMalloc](https://github.com/jeffhammond/sfmalloc)
* [SlimGuard](https://github.com/ssrg-vt/SlimGuard)
* [snmalloc](https://github.com/microsoft/snmalloc) and [paper here](https://dl.acm.org/doi/abs/10.1145/3315573.3329980).
* [SSMalloc: a low-latency, locality-conscious memory allocator with stable performance scalability](https://dl.acm.org/doi/10.1145/2349896.2349911)
* [streamflow](https://github.com/scotts/streamflow)
* [Supermalloc](https://github.com/kuszmaul/SuperMalloc)
* Thrifty-malloc
* [TCMalloc](https://github.com/google/tcmalloc) and [paper here](https://dl.acm.org/doi/10.1145/2618128.2618131).
* [TLSF](http://www.gii.upv.es/tlsf/)
* Ralloc: [Understanding and optimizing persistent memory allocation](https://dl.acm.org/doi/abs/10.1145/3332466.3374502).
* [VCMalloc](https://github.com/ycinhdj/vcmalloc)
* Traces of vmalloc in Apple's [ksh](https://opensource.apple.com/source/ksh/ksh-13/ksh/src/lib/libast/include/vmalloc.h.auto.html).
* [Vmalloc](https://doi.org/10.1002/(SICI)1097-024X(199603)26:3%3C357::AID-SPE15%3E3.0.CO;2-%23)
* [wfspan: Wait-free Dynamic Memory Management](https://dl.acm.org/doi/10.1145/3533724)
* [xmalloc](https://github.com/ederc/xmalloc)
* XMalloc

