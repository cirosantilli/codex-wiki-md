# mmap

↑ **Parent:** [Memory-mapped file](memory-mapped-file.md)

The [POSIX](posix.md) mapping interface. Ordinary [Linux kernel](linux-kernel.md) [file](computer-file.md) mappings require a positive length and an aligned [file offset](file-offset.md). A null address lets the [operating-system kernel](kernel-operating-system.md) choose an aligned base; length need not be aligned. Check for `MAP_FAILED`. After success the [file descriptor](file-descriptor.md) may be closed without invalidating the mapping; [munmap](munmap.md) or process termination removes it.[DESCRIPTION: address, length, offset and descriptor lifetime; munmap; RETURN VALUE](mmap-2-linux-manual-page.md)

Mapping does not extend the [backing file](backing-file.md). Under [POSIX](posix.md), for an initially partial last [memory page](memory-page.md), the tail beyond the [file](computer-file.md)'s end is zero-filled and is not written back as [file](computer-file.md) data; accesses to whole mapped [memory pages](memory-page.md) beyond the end raise `SIGBUS`. [POSIX](posix.md) leaves access to portions added or removed by later resizing unspecified. Establish the required [file](computer-file.md) size first and coordinate resizing with readers; a mapping's length is not proof that those [bytes](byte.md) exist in the [file](computer-file.md).[POSIX.1-2024, DESCRIPTION: partial end page, whole pages beyond the object, and changed file size; RATIONALE: references beyond the end do not extend the object](the-open-group-base-specifications-issue-8-ieee-std-1003-1-2024-by-ieee-and-others/mmap-posix-1-2024.md)

The [Linux kernel](linux-kernel.md) documents a tail-cache exception: modified beyond-end [bytes](byte.md) can survive in the [page cache](page-cache.md) and appear in later mappings, although never written to the [file](computer-file.md). Do not use that tail as reliable storage.[BUGS: modified contents beyond the object end can remain in the page cache](mmap-2-linux-manual-page.md)

**Table of contents**

- [munmap](munmap.md)

## ↑ Ancestors (5)

1. [Memory-mapped file](memory-mapped-file.md)
2. [Virtual memory](virtual-memory-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
