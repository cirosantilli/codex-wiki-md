# Page replacement

↑ **Parent:** [Paging](paging.md)

Choosing a resident [memory page](memory-page.md) to evict when another [memory page](memory-page.md) needs an occupied [page frame](page-frame.md). An unused [page frame](page-frame.md) needs no eviction. A [dirty memory page](dirty-memory-page.md) requires preservation before reuse, accounted for separately as [page writeback](page-writeback.md). A [page replacement](page-replacement.md) policy balances likely future reuse against the overhead of tracking past [memory references](memory-reference.md).

The opportunity comes from [temporal locality](temporal-locality.md): retaining a recently accessed [memory page](memory-page.md) can spare a later nonresident [page fault](page-fault.md). [Spatial locality](spatial-locality.md) helps consecutive accesses reuse the same [memory page](memory-page.md) until they cross its boundary. A [working set](working-set.md) describes recent demand, while the [resident set](resident-set.md) describes what is actually present. A small active footprint can fit in the available [page frames](page-frame.md) even when the whole [address space](address-space.md) cannot. These are useful workload tendencies, not guarantees about future [memory references](memory-reference.md).[Section 22.5, pp. 7–8, and the Types of Locality aside on p. 8: recent use motivates retention, but locality is a heuristic](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

The [page-reference trace](page-reference-trace.md) below uses the counterexample discussed in [Operating Systems: Three Easy Pieces by Remzi H. Arpaci-Dusseau and others](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others.md) (chapter 22, p. 5) and makes the decisions explicit. [FIFO page replacement](fifo-page-replacement.md) ranks arrival time, [LRU replacement](lru-replacement.md) ranks last access, [CLOCK page replacement](clock-page-replacement.md) samples recent use, and [optimal page replacement](optimal-page-replacement.md) knows the remaining [sequence](sequence.md) in advance. Count misses first; [page-replacement cost accounting](page-replacement-cost-accounting.md) separately counts [page writeback](page-writeback.md) and explains why fewer misses need not mean less total service time.

// Destination: computer-science.bigb

**Table of contents**

- [CLOCK page replacement](clock-page-replacement.md)
- [LRU replacement](lru-replacement.md)
  - [LRU stack property](lru-stack-property.md)
- [FIFO page replacement](fifo-page-replacement.md)
- [Page-reference trace](page-reference-trace.md)
- [Optimal page replacement](optimal-page-replacement.md)
- [Bélády's anomaly](belady-s-anomaly.md)
- [Dirty memory page](dirty-memory-page.md)
  - [Page writeback](page-writeback.md)
- [Page-replacement cost accounting](page-replacement-cost-accounting.md)

## ↑ Ancestors (5)

1. [Paging](paging.md)
2. [Virtual memory](virtual-memory.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Bélády's anomaly](belady-s-anomaly.md)
- [Copy-on-write page accounting](copy-on-write-page-accounting.md)
- [LRU replacement](lru-replacement.md)
- [Page fault](page-fault.md)
- [Page replacement](page-replacement.md)
- [Paging](paging.md)
- [Resident set](resident-set.md)
- [Thrashing (computer science)](thrashing-computer-science.md)
