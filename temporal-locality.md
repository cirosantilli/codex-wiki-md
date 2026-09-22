# Temporal locality

↑ **Parent:** [Computer science](computer-science-split.md)

Temporal locality is the tendency for the same item to be accessed again soon after an earlier access. For [computer memory](computer-memory.md), the item might be an [array](array-data-structure.md) element, a [cache line](cache-line.md) or a [memory page](memory-page.md); always specify the unit. [Temporal locality](temporal-locality.md) concerns reuse over time, whereas [spatial locality](spatial-locality.md) concerns accesses to nearby addresses. Both are properties of a workload, rather than guarantees about its next [memory reference](memory-reference.md). [Remzi H. Arpaci-Dusseau and Andrea C. Arpaci-Dusseau, Operating Systems: Three Easy Pieces, chapter 22, section 22.5 and the Types of Locality aside](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

For a worked example, let $A$ and $B$ denote two distinct [cache blocks](cache-line.md) at unrelated, nonadjacent [physical addresses](physical-address.md). An initially empty [fully associative cache](fully-associative-cache.md) holding two [cache lines](cache-line.md), with [LRU replacement](lru-replacement.md), receives the [sequence](sequence.md) $A,B,A$. The first $A$ causes a [cache miss](cache-miss.md) and leaves $A$ resident; $B$ causes another [cache miss](cache-miss.md) and leaves both $A$ and $B$ resident; the last $A$ is a [cache hit](cache-hit.md). [LRU replacement](lru-replacement.md) now regards $B$ as older than $A$. The benefit comes from [temporal locality](temporal-locality.md) of $A$, irrespective of how far apart the [cache blocks](cache-line.md) lie. With capacity one, the same [sequence](sequence.md) gives three [cache misses](cache-miss.md): reuse helps only if the item survives until it is needed.

The appealing idea is that a small [memory cache](cache-computing.md) can serve a large computation when its currently useful data stay small. Repeatedly reading a counter or executing the same instructions can exploit [temporal locality](temporal-locality.md). [LRU replacement](lru-replacement.md) and recency-based approximations try to retain recently used items. A [working set](working-set.md) records recent demand; if the active [working set](working-set.md) cannot fit in resident [memory pages](memory-page.md), [memory thrashing](thrashing-computer-science.md) can defeat this benefit. At [cache line](cache-line.md) granularity, even accesses to different [array](array-data-structure.md) elements can reuse the same [cache block](cache-line.md), as the [spatial locality](spatial-locality.md) example shows.

Peter J. Denning's May 1968 paper connected recent [memory page](memory-page.md) use to near-future demand through the [working set](working-set.md). Section 3 explicitly discusses the clustering of references to the same [memory page](memory-page.md) in time. This is a documented early treatment of the reasoning behind [temporal locality](temporal-locality.md), rather than a claim about who first coined the term. [Peter J. Denning, The Working Set Model for Program Behavior, Communications of the ACM 11(5), section 3: Definition and Properties, especially P2: Prediction](https://denninginstitute.com/pjd/PUBS/WSModel_1968.pdf)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Cache (computing)](cache-computing.md)
- [Cache hit](cache-hit.md)
- [FIFO page replacement](fifo-page-replacement.md)
- [Fully associative cache](fully-associative-cache.md)
- [LRU replacement](lru-replacement.md)
- [Optimal page replacement](optimal-page-replacement.md)
- [Page replacement](page-replacement.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/c/solution.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
- [Thrashing (computer science)](thrashing-computer-science.md)
- [Translation lookaside buffer](translation-lookaside-buffer.md)
- [Working set](working-set.md)
