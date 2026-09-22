# CLOCK page replacement

↑ **Parent:** [Page replacement](page-replacement.md)

Keep [page frames](page-frame.md) in a circular list with a reference [bit](bit.md) and a scanning hand. Clear set reference [bits](bit.md) while scanning; choose the first eligible [page frame](page-frame.md) with a clear reference [bit](bit.md). This second chance approximates [LRU replacement](lru-replacement.md) with cheaper tracking. When hardware reference flags are absent, revoking a mapping and handling its first later [page fault](page-fault.md) can supply a software reference observation.

For the [page-reference trace](page-reference-trace.md), number the three [page frames](page-frame.md) 1–3 and initially point the hand at 1. Every access sets the referenced [page frame](page-frame.md)'s reference [bit](bit.md) to 1. On a miss, scan from the hand: stop at an empty [page frame](page-frame.md) or a resident one with reference [bit](bit.md) 0; otherwise clear its reference [bit](bit.md) and advance cyclically. Install the requested [memory page](memory-page.md) with reference [bit](bit.md) 1 and advance the hand to the next [page frame](page-frame.md). Hits leave the hand where it is. This fixes a particular variant; clean-victim preference is excluded.[Section 22.8, p. 12: reference bits and the circular-hand algorithm; section 22.9, p. 13: dirty-page preference is an additional modification](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

After the first three accesses, all reference [bits](bit.md) are 1 and the hand is back at [page frame](page-frame.md) 1. Access 4 clears all three reference [bits](bit.md), returns to [page frame](page-frame.md) 1, evicts [memory page](memory-page.md) 1, installs [memory page](memory-page.md) 4, and leaves the hand at [page frame](page-frame.md) 2 with reference [bits](bit.md) $(1,0,0)$. This variant gives nine misses for three [page frames](page-frame.md) and ten for four on the displayed [sequence](sequence.md). Approximating [LRU replacement](lru-replacement.md) therefore does not inherit the [LRU stack property](lru-stack-property.md).

// Destination: computer-science.bigb

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [LRU stack property](lru-stack-property.md)
- [Page-reference trace](page-reference-trace.md)
- [Page replacement](page-replacement.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/c/solution.md)
