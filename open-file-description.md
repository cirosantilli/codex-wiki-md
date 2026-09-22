# Open file description

↑ **Parent:** [File descriptor](file-descriptor.md)

A record of an open access to a [file](computer-file.md), including its current position and access mode. Each [file descriptor](file-descriptor.md) reaches one [open file description](open-file-description.md), but several [file descriptors](file-descriptor.md) can share it. Separately opening the same ordinary [file](computer-file.md) creates separate [open file descriptions](open-file-description.md) with independent positions while still reaching the same [inode](inode.md). Thus [file descriptors](file-descriptor.md), [open file descriptions](open-file-description.md) and [hard links](hard-link.md) have different counts. [The Open Group, POSIX.1-2017, section 3.258: open file description](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_258)

// Target: computer-science.bigb

## ↑ Ancestors (5)

1. [File descriptor](file-descriptor.md)
2. [Process (computing)](process-computing.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Copy-on-write](copy-on-write.md)
- [File descriptor](file-descriptor.md)
- [File offset](file-offset.md)
- [File system](file-system.md)
- [Fork (system call)](fork-system-call.md)
- [Kernel (operating system)](kernel-operating-system.md)
- [Linux kernel](linux-kernel.md)
- [Open file description](open-file-description.md)
- [Unlinking an open file](unlinking-an-open-file.md)
