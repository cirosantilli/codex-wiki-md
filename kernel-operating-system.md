# Kernel (operating system)

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_(operating_system))

The [operating-system kernel](kernel-operating-system.md) is the core of an [operating system](operating-system.md), controlling access to resources and supplying mechanisms used by [operating-system processes](process-computing.md). [Processor privilege levels](processor-privilege-level.md) let it enforce boundaries that ordinary programs cannot simply overwrite. The [operating-system kernel](kernel-operating-system.md) connects [process scheduling](process-scheduling.md), [virtual memory](virtual-memory.md) and [file system](file-system.md) operations; a [system call](system-call.md) requests a service across that boundary. A [monolithic kernel](monolithic-kernel.md) and a [microkernel](microkernel.md) divide services differently, so the location of every [file system](file-system.md) service is a design choice.

For the toy [file system](file-system.md), opening `a` resolves its [directory entry](directory-entry.md) to [inode](inode.md) 42, establishes an [open file description](open-file-description.md), and returns [file descriptor](file-descriptor.md) `3`. Later reads use that [file descriptor](file-descriptor.md) to reach the existing [open file description](open-file-description.md), without resolving the spelling `a` again. This explains how [unlinking an open file](unlinking-an-open-file.md) preserves access: the open reference survives the [directory entry](directory-entry.md). The per-[operating-system process](process-computing.md) table interpreting `3` is maintained by the [operating-system kernel](kernel-operating-system.md); `3` itself is the small [integer](integer.md) passed by the program, not [inode](inode.md) 42. [The Open Group, POSIX.1-2024, open: file descriptor to open file description to file](https://pubs.opengroup.org/onlinepubs/9799919799/functions/open.html)

**Table of contents**

- [System call](system-call.md)
  - [Fork (system call)](fork-system-call.md)
- [Linux kernel](linux-kernel.md)
- [Monolithic kernel](monolithic-kernel.md)
- [Microkernel](microkernel.md)
  - [Microkernel file-read example](microkernel-file-read-example.md)
  - [Microkernel service failure isolation](microkernel-service-failure-isolation.md)
  - [Microkernel communication cost](microkernel-communication-cost.md)
  - [seL4](sel4.md)
    - [seL4 verification scope](sel4-verification-scope.md)
- [Kernel preemption](kernel-preemption.md)

## ↑ Ancestors (3)

1. [Operating system](operating-system.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)
