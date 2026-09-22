# Memory-mapped file

↑ **Parent:** [Virtual memory](virtual-memory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memory-mapped_file)

A [memory-mapped file](memory-mapped-file.md) makes a range of a [file](computer-file.md) accessible through an [operating-system process](process-computing.md)'s [virtual memory](virtual-memory-split.md) [address space](address-space.md). Once the mapping exists, ordinary loads and stores address its contents instead of explicitly reading them into a separate application buffer. This is attractive for jumping between records in a large [file](computer-file.md): an offset becomes an address calculation, and [demand paging](demand-paging.md) can supply the needed [memory pages](memory-page.md). It removes the application's explicit read-and-copy step; it does not promise that every access avoids copying, [input-output](input-output.md), [page faults](page-fault.md) or overhead, or that mapping is universally faster.

The [backing file](backing-file.md), [page cache](page-cache.md) contents and each [operating-system process](process-computing.md)'s [page table](page-table.md) play different roles. For ordinary buffered [Linux kernel](linux-kernel.md) mappings, the [page cache](page-cache.md) holds reusable [file](computer-file.md) contents; normal reads and writes also use it. A valid mapping can exist before this [operating-system process](process-computing.md) has a usable [page table entry](page-table-entry.md). A first load can therefore trigger a [page fault](page-fault.md) even when another reader has already brought the contents into [computer memory](computer-memory.md). If the contents are absent, servicing the [page fault](page-fault.md) can require [input-output](input-output.md); if present, the handler can install an [address translation](address-translation.md) without that read. Special paths that bypass the [page cache](page-cache.md) are outside this explanation.[Page Cache, opening paragraph: normal reads, writes and mmaps go through the page cache; bypass paths exist](page-cache-by-the-kernel-development-community.md)

The following example and diagrams are an original toy model, not an actual benchmark or a trace of a running [operating system](operating-system-split.md). They assume ordinary buffered [file](computer-file.md) mappings, successful accesses, two cooperating [operating-system processes](process-computing.md), no concurrent resizing, and explicitly ordered actions. [Memory-mapped file offset translation](memory-mapped-file-offset-translation.md) explains where the accesses land; [shared file mappings](shared-file-mapping.md) and [private file mappings](private-file-mapping.md) explain whose contents change; [memory-mapped file synchronization](memory-mapped-file-synchronization.md) explains the separate persistence boundary.

**Table of contents**

- [Backing file](backing-file.md)
- [mmap](mmap.md)
  - [munmap](munmap.md)
- [Memory-mapped file offset translation](memory-mapped-file-offset-translation.md)
- [Shared file mapping](shared-file-mapping.md)
- [Private file mapping](private-file-mapping.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
  - [msync](msync.md)

## ↑ Ancestors (4)

1. [Virtual memory](virtual-memory-split.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Backing file](backing-file.md)
- [Copy-on-write](copy-on-write.md)
- [Copy-on-write fault handling](copy-on-write-fault-handling.md)
- [File offset](file-offset.md)
- [Memory-mapped file](memory-mapped-file.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/d/solution.md)
- [Unlinking an open file](unlinking-an-open-file.md)
