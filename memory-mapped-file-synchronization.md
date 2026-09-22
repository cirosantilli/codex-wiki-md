# Memory-mapped file synchronization

↑ **Parent:** [Memory-mapped file](memory-mapped-file.md)

There are two distinct questions: whether another [operating-system process](process-computing.md) can observe shared contents, and whether those contents survive a crash. In the timeline, persistent storage deliberately remains $(7,8)$ while the shared [page cache](page-cache.md) contains $(11,12)$. No background [page writeback](page-writeback.md) occurs in this toy interval. Real [page writeback](page-writeback.md) may persist some contents earlier; shared visibility alone cannot tell the reader which contents are durable.

For the covered shared range, `msync(base, length, MS_SYNC)` requests [page writeback](page-writeback.md) and waits for completion; check its return value. `MS_ASYNC` is not a durable completion acknowledgment, and on modern [Linux kernel](linux-kernel.md) versions it is a no-op because dirty contents are already tracked. The address must be aligned, so synchronizing our changed second page uses `base + 4096`, length 4096, rather than `base + 4133`. Unmapping alone is not a guarantee of completed writeback.[DESCRIPTION, RETURN VALUE, ERRORS and VERSIONS: covered range, MS\_SYNC versus MS\_ASYNC, page-aligned address, and Linux MS\_ASYNC behavior since 2.6.19](msync-2-linux-manual-page-by-linux-man-pages-project.md)

For persistence of the [file](computer-file.md) and associated [file metadata](file-metadata.md), [fsync](fsync.md) on an open [file descriptor](file-descriptor.md) is a broader interface; a new [directory entry](directory-entry.md) needs separate synchronization of its [file-system directory](file-system-directory.md). Retain a suitable [file descriptor](file-descriptor.md) if the persistence protocol needs it after mapping. Successful storage completion still relies on the [file system](file-system-split.md) and device honoring their persistence contracts.[DESCRIPTION, RETURN VALUE and ERRORS: file data and metadata, directory entry, completion and reported failures](fsync-2-linux-manual-page-by-linux-man-pages-project.md)

Neither [fsync](fsync.md) nor [msync](msync.md) supplies [mutual exclusion](mutual-exclusion.md), an [atomic storage write](atomic-storage-write.md) for several [memory pages](memory-page.md), or an application-wide [file-system transaction](file-system-transaction.md). Stop or coordinate writers before deciding which update a completion acknowledges. A crash during [page writeback](page-writeback.md) can leave a mixture of old and new contents unless a separate recovery protocol provides [file-system crash consistency](file-system-crash-consistency.md). The last timeline row assumes successful synchronous completion, honored [storage flush](storage-flush.md) semantics and no subsequent writer; it illustrates a persistence boundary, not a promise about arbitrary hardware failures.

**Table of contents**

- [msync](msync.md)

## ↑ Ancestors (5)

1. [Memory-mapped file](memory-mapped-file.md)
2. [Virtual memory](virtual-memory-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Memory-mapped file](memory-mapped-file.md)
- [msync](msync.md)
- [munmap](munmap.md)
