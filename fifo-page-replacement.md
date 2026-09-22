# FIFO page replacement

↑ **Parent:** [Page replacement](page-replacement.md)

Evict the [memory page](memory-page.md) loaded earliest among currently resident [memory pages](memory-page.md), without refreshing its position on access. It is simple but ignores [temporal locality](temporal-locality.md) and can evict a frequently accessed [memory page](memory-page.md).

Implement this ranking with a [FIFO queue](fifo-queue.md) of resident [memory pages](memory-page.md): append on loading, remove the oldest on eviction, and leave the queue unchanged on a hit. [Belady anomaly](belady-s-anomaly.md) shows why preserving arrival order can give more misses with more [page frames](page-frame.md). The comparison uses the same [page-reference trace](page-reference-trace.md) and empty initial [resident sets](resident-set.md) in both runs.[Section 22.3, pp. 4–5: FIFO ordering; Belady's Anomaly aside, p. 5: the twelve-reference counterexample and contrast with stack policies](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

**Table of contents**

- [FIFO cache](fifo-cache.md)

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Bélády's anomaly](belady-s-anomaly.md)
- [LRU replacement](lru-replacement.md)
- [Page-reference trace](page-reference-trace.md)
- [Page replacement](page-replacement.md)
- [Page-replacement cost accounting](page-replacement-cost-accounting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/c/solution.md)
