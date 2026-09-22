# Buffer cache writeback

↑ **Parent:** [Buffer cache](buffer-cache.md)

Transferring a [dirty buffer](dirty-buffer.md)'s current contents to its backing location. The [buffer cache state model](buffer-cache-state-model.md) permits no concurrent modification during the transfer and marks the result clean only after successful completion. A failed write preserves the obligation and prevents the proposed [buffer cache eviction](buffer-cache-eviction.md). A production implementation allowing new writes during [input-output](input-output.md) must retain their obligation rather than incorrectly clearing it when an older transfer finishes.

A successful transfer can leave data in a device's volatile [memory cache](cache-computing.md). A [storage flush](storage-flush.md) or the documented equivalent supplies a persistence boundary; [file-system journaling](file-system-journaling.md) supplies recovery rules for related updates. These are additional obligations, not consequences of becoming a [clean buffer](clean-buffer.md).[Explicit volatile write back cache control by The kernel development community](explicit-volatile-write-back-cache-control-by-the-kernel-development-community.md)

## ↑ Ancestors (5)

1. [Buffer cache](buffer-cache.md)
2. [File system](file-system-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Buffer cache](buffer-cache.md)
- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Dirty buffer](dirty-buffer.md)
- [Page cache](page-cache.md)
- [Page writeback](page-writeback.md)
- [xv6 buffer cache](xv6-buffer-cache.md)
