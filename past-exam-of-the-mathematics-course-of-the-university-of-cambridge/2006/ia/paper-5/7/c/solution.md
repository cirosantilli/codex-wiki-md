<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Use LRU replacement, or a modest recency-based approximation, for eligible buffer-cache entries.** Unlike individual memory accesses, [buffer cache](../../../../../../buffer-cache.md) lookups already pass through [operating system](../../../../../../operating-system.md) code. Updating an [LRU replacement](../../../../../../lru-replacement.md) list on each lookup is therefore practical: remove the accessed entry from its old position and put it at the most-recent end; choose the oldest unpinned entry as victim. A hash lookup plus a doubly linked recency list makes this bookkeeping constant time.

Good [temporal locality](../../../../../../temporal-locality.md) favors retaining recently used blocks. [FIFO page replacement](../../../../../../fifo-page-replacement.md)'s arrival-only criterion can evict a block used moments ago. [CLOCK page replacement](../../../../../../clock-page-replacement.md) can save bookkeeping, but the difficulty of observing arbitrary memory references that motivates it is absent for software-mediated block accesses. Dirty victims require write-back, so a policy can favor an old clean buffer or arrange background cleaning without discarding recent hot data. A long one-pass scan can pollute pure [LRU replacement](../../../../../../lru-replacement.md); scan-resistant variants are useful refinements rather than a reason to ignore recency altogether.

## ↑ Ancestors (11)

1. [C](../c.md)
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
