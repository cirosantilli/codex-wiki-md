# Page cache

↑ **Parent:** [Buffer cache](buffer-cache.md)

Caching [file](computer-file.md) contents in units based on [memory pages](memory-page.md), commonly by a [file](computer-file.md) mapping and an offset, rather than necessarily by the device-and-block [buffer cache key](buffer-cache-key.md) used above. A [file](computer-file.md)'s offset must be mapped to storage before device access; the two naming systems describe different layers. How [page cache](page-cache.md) and [buffer cache](buffer-cache.md) storage relate depends on the [operating system](operating-system.md) and [file system](file-system.md). A separate duplicate copy at each layer is not a universal requirement.

For the [Linux kernel](linux-kernel.md) interfaces documented in [Buffer Heads by The kernel development community](buffer-heads-by-the-kernel-development-community.md), per-block state can be attached to larger cached memory units called [Linux folios](linux-folio.md); `mark_buffer_dirty` also marks the backing page dirty in the [page cache](page-cache.md). The documented reclamation checks include dirty state, pending [buffer cache writeback](buffer-cache-writeback.md) and elevated reference counts. That documentation deprecates [Linux buffer heads](linux-buffer-head.md) for new [file systems](file-system.md) in favour of [iomap](iomap.md). These are platform-specific interfaces, not a definition that every [page cache](page-cache.md) has [Linux buffer heads](linux-buffer-head.md) or that every [buffer cache](buffer-cache.md) has its own disjoint allocation. [Buffer Heads by The kernel development community](buffer-heads-by-the-kernel-development-community.md)

**Table of contents**

- [Linux buffer head](linux-buffer-head.md)
- [Linux folio](linux-folio.md)
- [iomap](iomap.md)

## ↑ Ancestors (5)

1. [Buffer cache](buffer-cache.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Memory-mapped file](memory-mapped-file.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
- [mmap](mmap.md)
- [Page cache](page-cache.md)
- [Private file mapping](private-file-mapping.md)
- [Shared file mapping](shared-file-mapping.md)
