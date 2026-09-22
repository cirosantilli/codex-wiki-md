# File descriptor

↑ **Parent:** [Process (computing)](process-computing.md)

A nonnegative [integer](integer-split.md) identifying an open access in one [operating-system process](process-computing.md). The program passes its value to operations such as reading and closing; the [operating-system kernel](kernel-operating-system.md) interprets it through that [operating-system process](process-computing.md)'s descriptor table. In the toy example, table entry `3` refers to an [open file description](open-file-description.md) for [inode](inode.md) 42. Another [operating-system process](process-computing.md)'s entry `3` can reach a different [file](computer-file.md), and a closed [file descriptor](file-descriptor.md) value can be reused. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 39, section 39.3: per-process file descriptors](https://pages.cs.wisc.edu/~remzi/OSTEP/file-intro.pdf)

**Table of contents**

- [Open file description](open-file-description.md)

## ↑ Ancestors (4)

1. [Process (computing)](process-computing.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Copy-on-write](copy-on-write.md)
- [File descriptor](file-descriptor.md)
- [File system](file-system-split.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [Fork (system call)](fork-system-call.md)
- [Kernel (operating system)](kernel-operating-system.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
- [mmap](mmap.md)
- [munmap](munmap.md)
- [Open file description](open-file-description.md)
- [Operating system](operating-system-split.md)
- [POSIX](posix.md)
- [Process (computing)](process-computing.md)
- [Thread (computing)](thread-computing.md)
- [Unlinking an open file](unlinking-an-open-file.md)
