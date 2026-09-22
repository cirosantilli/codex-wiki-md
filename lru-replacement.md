# LRU replacement

↑ **Parent:** [Page replacement](page-replacement.md)

Evict the least recently accessed eligible item. Exact recency tracking on every [memory reference](memory-reference.md) can be expensive, whereas accesses to a [buffer cache](buffer-cache.md) already pass through software. Recency captures [temporal locality](temporal-locality.md) but a long scan can evict frequently reused items before their next use.

For [page replacement](page-replacement.md), update recency on hits as well as misses; evict only when a miss requires a [page frame](page-frame.md) and all eligible [page frames](page-frame.md) are occupied. The four-page cycle in [memory thrashing](thrashing-computer-science.md) shows how exact [LRU replacement](lru-replacement.md) behaves at capacities three and four.[Chapter 22, section 22.5, pp. 7–8: least-recently-used eviction; section 22.7, p. 11: update recency on every access](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

The [LRU stack property](lru-stack-property.md) compares different capacities on one fixed [page-reference trace](page-reference-trace.md); it does not say that [LRU replacement](lru-replacement.md) always beats [FIFO page replacement](fifo-page-replacement.md). On the displayed [sequence](sequence.md), three-[page frame](page-frame.md) [LRU replacement](lru-replacement.md) has ten misses, versus nine for [FIFO page replacement](fifo-page-replacement.md), while four-[page frame](page-frame.md) [LRU replacement](lru-replacement.md) has only eight.

**Table of contents**

- [LRU cache](lru-cache.md)
- [LRU stack property](lru-stack-property.md)

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Cache (computing)](cache-computing.md)
- [Cache miss](cache-miss.md)
- [Capacity miss](capacity-miss.md)
- [CLOCK page replacement](clock-page-replacement.md)
- [Conflict miss](conflict-miss.md)
- [Fully associative cache](fully-associative-cache.md)
- [LRU cache](lru-cache.md)
- [LRU replacement](lru-replacement.md)
- [LRU stack property](lru-stack-property.md)
- [Page-reference trace](page-reference-trace.md)
- [Page replacement](page-replacement.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/c/solution.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
- [Thrashing (computer science)](thrashing-computer-science.md)
- [Working set](working-set.md)
