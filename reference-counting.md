# Reference counting

↑ **Parent:** [Computer memory](computer-memory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reference_counting)

Tracking how many references retain an object. For the [copy-on-write](copy-on-write.md) model, the object is a [page frame](page-frame.md) and each mapping retains it; removing the last reference permits reclamation. Real [operating-system kernels](kernel-operating-system.md) can track other kinds of ownership too. [Lab: Copy-on-Write Fork for xv6](6-1810-and-fall-2022/lab-copy-on-write-fork-for-xv6.md)

## ↑ Ancestors (3)

1. [Computer memory](computer-memory.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Copy-on-write](copy-on-write.md)
- [Copy-on-write fault handling](copy-on-write-fault-handling.md)
- [Linux buffer head](linux-buffer-head.md)
- [Pinned buffer](pinned-buffer.md)
