# Buffer cache

↑ **Parent:** [File system](file-system-split.md)

A memory cache of device blocks indexed by device identity and block number. A hit avoids slow device access; a miss obtains a buffer and reads the block. Dirty buffers carry modified data that must be written before reuse, and pinned buffers cannot be evicted while an operation uses them. Deferred writes improve throughput but need explicit durability handling.

A [buffer cache](buffer-cache.md) can hold both [file data blocks](file-data-block.md) and storage containing [file metadata](file-metadata.md), such as [inodes](inode.md) and [block allocation bitmaps](block-allocation-bitmap.md). Reusing a [buffered device block](buffered-device-block.md) saves repeated [input-output](input-output.md); retaining several modifications before [buffer cache writeback](buffer-cache-writeback.md) can combine them into one transfer. Section 40.7 of [Operating Systems: Three Easy Pieces by Remzi H. Arpaci-Dusseau and others](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others.md) explains these benefits for [file systems](file-system-split.md).[pp. 14–16: caching and buffering](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/file-system-implementation.md)

The central distinction is that a [dirty buffer](dirty-buffer.md) needs a write, whereas a [pinned buffer](pinned-buffer.md) must retain its identity. A [clean buffer](clean-buffer.md) can still be pinned, and a [dirty buffer](dirty-buffer.md) can have no client references. Neither releasing a reference nor obtaining a [cache hit](cache-hit.md) establishes [file-system transaction durability](file-system-transaction-durability.md).

**Table of contents**

- [Buffered device block](buffered-device-block.md)
  - [Buffer cache key](buffer-cache-key.md)
  - [Buffer cache validity](buffer-cache-validity.md)
  - [Dirty buffer](dirty-buffer.md)
  - [Clean buffer](clean-buffer.md)
  - [Pinned buffer](pinned-buffer.md)
- [Buffer cache writeback](buffer-cache-writeback.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Buffer cache state model](buffer-cache-state-model.md)
  - [Buffer cache access trace](buffer-cache-access-trace.md)
- [xv6 buffer cache](xv6-buffer-cache.md)
- [Page cache](page-cache.md)
  - [Linux buffer head](linux-buffer-head.md)
  - [Linux folio](linux-folio.md)
  - [iomap](iomap.md)

## ↑ Ancestors (4)

1. [File system](file-system-split.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Buffer cache](buffer-cache.md)
- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache key](buffer-cache-key.md)
- [Cache (computing)](cache-computing.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [LRU replacement](lru-replacement.md)
- [Page cache](page-cache.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/c/solution.md)
