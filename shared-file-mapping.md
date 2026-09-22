# Shared file mapping

↑ **Parent:** [Memory-mapped file](memory-mapped-file.md)

With `MAP_SHARED`, updates are visible to other [operating-system processes](process-computing.md) mapping the same region and are carried through to the [backing file](backing-file.md). With `MAP_PRIVATE`, updates instead stay private, and later [backing file](backing-file.md) changes have unspecified visibility in that mapping.[DESCRIPTION, The flags argument: MAP\_SHARED and MAP\_PRIVATE](mmap-2-linux-manual-page.md)

In the toy model, both [shared file mappings](shared-file-mapping.md) initially read backing [bytes](byte.md) $x=7,y=8$ at [file offsets](file-offset.md) 8229 and 8230. Both [memory pages](memory-page.md) have been accessed, so their translations are installed. A shared store changes the common [page cache](page-cache.md) contents and creates a [dirty memory page](dirty-memory-page.md) eligible for [page writeback](page-writeback.md). That change can be observed before it reaches persistent storage. Cooperating readers need [synchronization](synchronization-computing.md) to know when an update is ready; `MAP_SHARED` alone supplies no [mutual exclusion](mutual-exclusion.md) or indivisible multi-field update.

## ↑ Ancestors (5)

1. [Memory-mapped file](memory-mapped-file.md)
2. [Virtual memory](virtual-memory-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Memory-mapped file](memory-mapped-file.md)
- [Memory-mapped file offset translation](memory-mapped-file-offset-translation.md)
- [Private file mapping](private-file-mapping.md)
- [Shared file mapping](shared-file-mapping.md)
