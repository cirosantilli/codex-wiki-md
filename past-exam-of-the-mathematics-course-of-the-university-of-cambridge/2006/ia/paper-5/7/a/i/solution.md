<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[FIFO page replacement](../../../../../../../fifo-page-replacement.md) orders resident pages by when they were loaded and evicts the oldest arrival. An access to a resident page does not change this order, so an old but heavily used page can be the next victim.

[LRU replacement](../../../../../../../lru-replacement.md) records the recency of every page access and evicts the page whose most recent access is oldest. It makes use of [temporal locality](../../../../../../../temporal-locality.md), but exact reference tracking can require expensive per-access hardware or software bookkeeping.

[CLOCK page replacement](../../../../../../../clock-page-replacement.md) arranges frames in a circle with a scanning hand and one reference flag per frame. A use sets the flag. During replacement, the hand clears a set flag and moves on, giving that page another chance; it selects an eligible frame with a clear flag. Recent pages tend to survive a scan. [CLOCK page replacement](../../../../../../../clock-page-replacement.md) approximates recency rather than preserving the exact [LRU replacement](../../../../../../../lru-replacement.md) ordering. A dirty victim must be written back before its frame is reused, and pinned frames must be skipped.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
