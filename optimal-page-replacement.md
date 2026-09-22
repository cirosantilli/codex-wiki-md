# Optimal page replacement

↑ **Parent:** [Page replacement](page-replacement.md)

On a miss with all [page frames](page-frame.md) occupied, evict the resident [memory page](memory-page.md) whose next access is farthest in the remaining [page-reference trace](page-reference-trace.md). Treat no further access as farther than any finite next-use index; in the diagram, ties choose the lowest-numbered [page frame](page-frame.md). This is an offline, clairvoyant benchmark: a general [operating system](operating-system-split.md) cannot know its future [memory references](memory-reference.md). It minimizes miss count in the stated fixed-capacity [demand paging](demand-paging.md) model, rather than predicting the future from [temporal locality](temporal-locality.md).[Section 22.2, pp. 2–4: farthest-future MIN policy, minimum misses, and the unavailable-future limitation](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

In the [page-reference trace](page-reference-trace.md), seven misses with three [page frames](page-frame.md) is therefore a lower bound for any policy using the same assumptions; with four [page frames](page-frame.md) the corresponding minimum is six. The benchmark is useful for judging how much improvement is possible on a recorded workload. Its objective counts each miss equally. Different [page writeback](page-writeback.md) costs or unequal loading costs require a different objective; minimum misses alone does not prove minimum elapsed time.

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Page-reference trace](page-reference-trace.md)
- [Page replacement](page-replacement.md)
- [Page-replacement cost accounting](page-replacement-cost-accounting.md)
