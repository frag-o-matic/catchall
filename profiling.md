### Memory

Overview: [1](https://stackoverflow.com/questions/63166/how-to-determine-cpu-and-memory-consumption-from-inside-a-process)
[2](http://elinux.org/Runtime_Memory_Measurement)

#### Stack

[checkstack.pl](http://www.kegel.com/stackcheck/#static) -> calc stack usage of funcs, **does NOT** handle recusive stuff and `alloca()`

[fstack-usage](https://gcc.gnu.org/onlinedocs/gnat_ugn/Static-Stack-Usage-Analysis.html), `gcc-4.6` onwards. Tutorial [here](https://mcuoneclipse.com/2015/08/21/gnu-static-stack-usage-analysis/)

[StackAnalyzer](https://www.absint.com/stackanalyzer/) -> paid, supports only specific IDEs (???)

#### Heap & Dynamic

[massif](http://valgrind.org/docs/manual/ms-manual.html) -> part of Valgrind suite, can also check stack mem, but is sloooow. Simple [visualizer](https://sourceforge.net/projects/massiftool/)

[heaptrack](http://milianw.de/blog/heaptrack-a-heap-memory-profiler-for-linux) 

#### Overall Runtime Usage

[top](http://man7.org/linux/man-pages/man1/top.1.html)

[ps](https://linux.die.net/man/1/ps)

[pmap](https://linux.die.net/man/1/pmap)

[smem](https://linux.die.net/man/8/smem)

### Time

Overview [1](http://gernotklingler.com/blog/gprof-valgrind-gperftools-evaluation-tools-application-level-cpu-profiling-linux/)
[2](www.linuxjournal.com/article/2622)
[3](http://www.visitusers.org/index.php?title=Profiling)

[callgrind](http://valgrind.org/docs/manual/cl-manual.html) -> part of Valgrind suite

[gprof](https://web.eecs.umich.edu/~sugih/pointers/gprof_quick.html) -> GNU profiler (part of `binutils`)

[gperftools](https://github.com/gperftools/gperftools) -> Google's profiler

[oprofile](http://oprofile.sourceforge.net/news/)

[sprof](http://man7.org/linux/man-pages/man1/sprof.1.html) part of `libc` & used for profiling shared libraries where `gprof` doesn't work. Example [here](https://stackoverflow.com/questions/881074/how-to-use-sprof) and [here](https://greg-n-blog.blogspot.in/2010/01/profiling-shared-library-on-linux-using.html)

### I/O

Overview [1](http://www.linuxprogrammingblog.com/io-profiling)
[2](http://www.slashroot.in/linux-system-io-monitoring)

[iotop](https://linux.die.net/man/1/iotop)

[iostat](https://linux.die.net/man/1/iostat)

[ioprof](https://github.com/01org/ioprof)

**TODO: Add network profilers**

### Locks & IPC

[ipcs](http://man7.org/linux/man-pages/man1/ipcs.1.html) with examples [here](http://www.thegeekstuff.com/2010/08/ipcs-command-examples/) -> not really a profiler ;-)

### Binary sizes

`nm --print-size --size-sort --radix=d whatever.o` -> size of functions and statics, from [here](http://stackoverflow.com/a/11720779)

`size -A -d whatever.o` -> size of various sections, from [here](http://stackoverflow.com/a/11720779)

`readelf -e whatever.o` -> size of various sections, from [here](http://stackoverflow.com/a/11723398)

`objdump` -> see [here](http://www.sanfoundry.com/objdump-command-usage-examples-in-linux/) and [here](http://www.thegeekstuff.com/2012/09/objdump-examples) for examples

