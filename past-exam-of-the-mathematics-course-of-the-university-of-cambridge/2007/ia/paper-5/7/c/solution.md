<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Paging](../../../../../../paging.md) divides a virtual address space into fixed-size pages mapped independently to fixed-size physical frames. It avoids external fragmentation of physical memory, although the last page of an allocation can contain unused space. Pages are principally allocation units and need not coincide with meaningful program objects.

[Memory segmentation](../../../../../../memory-segmentation.md) instead presents logical variable-sized regions such as code, a stack or a data object. An address contains a segment identifier and an offset; a segment descriptor gives a base, limit and permissions. The offset is checked against the limit. Pure contiguous physical segmentation can suffer external fragmentation and may need relocation or compaction, but its object-level boundaries aid protection and sharing.

Combine the two by mapping a segment offset to a linear virtual address and then using [paging](../../../../../../paging.md) for physical allocation, or by having each segment descriptor refer to its own [page table](../../../../../../page-table.md). Cache descriptors and translations so ordinary references do not repeatedly traverse all tables. Segment pages may occupy noncontiguous frames, while bounds and rights remain defined at segment granularity. **Segmentation supplies logical objects and bounds; paging supplies efficient noncontiguous physical storage.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
