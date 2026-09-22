<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Emulate reference observations using [page table](../../../../../../../page-table.md) protection and [page faults](../../../../../../../page-fault.md). When resetting a page's reference state, temporarily revoke access to its resident mapping and invalidate any corresponding [translation lookaside buffer](../../../../../../../translation-lookaside-buffer.md) entry. The first subsequent access traps. The handler recognizes an intentionally protected resident page, sets a software reference flag and restores the mapping without performing a disk read. A later [CLOCK page replacement](../../../../../../../clock-page-replacement.md) scan can use and clear this software flag.

**One protection fault records the first access after each reset**, rather than trapping on every access. All mappings that can access the frame must be considered. The method requires ordinary memory-protection traps, even though hardware reference bits are absent, and adds a fault cost that native reference flags avoid.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
