# Buffered device block

↑ **Parent:** [Buffer cache](buffer-cache.md)

A [data structure](data-structure-split.md) holding the contents of one fixed-size region of a storage device, together with its [buffer cache key](buffer-cache-key.md), [buffer cache validity](buffer-cache-validity.md), modification state and lifetime information. A storage region containing [file metadata](file-metadata.md) is just as eligible as a [file data block](file-data-block.md). The structure can survive many callers: releasing it usually makes it available for later reuse, rather than immediately deleting the cached contents.

**Table of contents**

- [Buffer cache key](buffer-cache-key.md)
- [Buffer cache validity](buffer-cache-validity.md)
- [Dirty buffer](dirty-buffer.md)
- [Clean buffer](clean-buffer.md)
- [Pinned buffer](pinned-buffer.md)

## ↑ Ancestors (5)

1. [Buffer cache](buffer-cache.md)
2. [File system](file-system-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Buffer cache](buffer-cache.md)
- [Buffer cache key](buffer-cache-key.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Buffer cache validity](buffer-cache-validity.md)
- [Clean buffer](clean-buffer.md)
- [Dirty buffer](dirty-buffer.md)
- [Page writeback](page-writeback.md)
- [Pinned buffer](pinned-buffer.md)
