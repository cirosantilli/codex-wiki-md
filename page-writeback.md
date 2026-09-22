# Page writeback

↑ **Parent:** [Dirty memory page](dirty-memory-page.md)

Preserving the modified contents of a [dirty memory page](dirty-memory-page.md) in its backing storage. The reference model waits for successful [page writeback](page-writeback.md) before reusing the victim's [page frame](page-frame.md); failure cannot authorize losing its modifications. A reference [bit](bit.md) records recent access, while the dirty flag records a write obligation: reading can set the first without setting the second. [Buffer cache writeback](buffer-cache-writeback.md) concerns the analogous obligation for a [buffered device block](buffered-device-block.md).

## ↑ Ancestors (7)

1. [Dirty memory page](dirty-memory-page.md)
2. [Page replacement](page-replacement.md)
3. [Paging](paging.md)
4. [Virtual memory](virtual-memory.md)
5. [Operating system](operating-system.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Dirty memory page](dirty-memory-page.md)
- [LRU stack property](lru-stack-property.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
- [Optimal page replacement](optimal-page-replacement.md)
- [Page replacement](page-replacement.md)
- [Page-replacement cost accounting](page-replacement-cost-accounting.md)
- [Page writeback](page-writeback.md)
- [Private file mapping](private-file-mapping.md)
- [Shared file mapping](shared-file-mapping.md)
