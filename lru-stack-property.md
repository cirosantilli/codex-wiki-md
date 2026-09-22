# LRU stack property

↑ **Parent:** [LRU replacement](lru-replacement.md)

For exact [LRU replacement](lru-replacement.md), let $R_k(t)$ be the [resident set](resident-set.md) after the first $t$ accesses of a fixed [page-reference trace](page-reference-trace.md) with capacity $k$. With empty starts, identical access order, freely placeable [memory pages](memory-page.md), and all resident [memory pages](memory-page.md) eligible for eviction,

$$
R_k(t)\subseteq R_{k+1}(t)\qquad\text{for every }t\geq0.
$$

Here $\subseteq$ means [subset](subset.md). At every time, form one capacity-independent ordered list of distinct [memory pages](memory-page.md), most recently accessed first. An access moves its [memory page](memory-page.md) to the front, preserving the order of the others. Exact [LRU replacement](lru-replacement.md) with $k$ [page frames](page-frame.md) retains the first $k$ entries, or all entries if fewer than $k$ have appeared. The first $k$ entries are contained in the first $k+1$, proving the property. This recency list is not the push/pop interface of a [LIFO stack](stack-data-structure.md).[Belady's Anomaly aside, p. 5: stack-property inclusion and its consequence for LRU; section 22.7, p. 11: exact recency must be updated on every access](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

Apply inclusion immediately before an access: a hit with $k$ [page frames](page-frame.md) must also hit with $k+1$. Thus cumulative misses with $k+1$ cannot exceed those with $k$, at any prefix of the same [page-reference trace](page-reference-trace.md). On the displayed [sequence](sequence.md), the counts decrease from ten to eight when capacity increases from three to four. Arbitrary initial contents, different access orders, protected victims, or clean-victim preference fall outside the proof. Nor does it prove monotonic [page writeback](page-writeback.md) costs, or apply automatically to [CLOCK page replacement](clock-page-replacement.md) just because that policy approximates [LRU replacement](lru-replacement.md).

// Destination: computer-science.bigb

## ↑ Ancestors (7)

1. [LRU replacement](lru-replacement.md)
2. [Page replacement](page-replacement.md)
3. [Paging](paging.md)
4. [Virtual memory](virtual-memory.md)
5. [Operating system](operating-system.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [CLOCK page replacement](clock-page-replacement.md)
- [LRU replacement](lru-replacement.md)
