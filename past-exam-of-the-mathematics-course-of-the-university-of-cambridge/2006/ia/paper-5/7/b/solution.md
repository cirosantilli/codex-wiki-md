<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [buffer cache](../../../../../../buffer-cache.md) keeps copies of device blocks in main memory, indexed by device identity and block number. It reduces expensive repeated device reads and can combine several modifications into one write. It also gives software a controlled place to hold data while requests are in progress.

On a read, the [operating system](../../../../../../operating-system.md) looks up the block. A valid cached copy gives a hit and supplies the data; a miss reserves an eligible buffer, writes its old contents first if dirty, issues the device read, and marks the new contents valid when the transfer completes. A write modifies the buffer and marks it dirty. Under a write-back policy, a later flush or eviction sends it to the device; under write-through, completion also waits for the required device write. Dirty state differs from “currently in use”: a pinned or locked buffer cannot simply be reused while a request depends on it.

A [buffer cache](../../../../../../buffer-cache.md) needs synchronization for concurrent readers, writers and in-flight transfers, and should avoid inconsistent independent copies of the same block. Explicit flushes and ordering are needed when durable storage is required; caching alone does not guarantee that an acknowledged in-memory update survives a crash. Replacement chooses among eligible buffers, preserving dirty data before reuse.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
