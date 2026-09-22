<h1 id="2/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The logical [file data block](../../../../../../file-data-block.md) index and within-block [file offset](../../../../../../file-offset.md) are

$$
2^{24}+20000=8201\cdot2048+1568.
$$

Direct pointers cover logical indices 0 through 9. The singly indirect region covers 10 through $10+512-1=521$. The requested [file data block](../../../../../../file-data-block.md) therefore lies in the doubly indirect region, at relative index

$$
8201-(10+512)=7679=14\cdot512+511.
$$

Follow the doubly [indirect block pointer](../../../../../../indirect-block-pointer.md) in the [inode](../../../../../../inode.md), read its top address block and select entry 14, read that second address block and select entry 511, then read the resulting [file data block](../../../../../../file-data-block.md) and take byte offset 1568. These entry indices are zero-based.

$$
\boxed{3\text{ block reads: two address blocks and one data block}.}
$$

This assumes a resident [inode](../../../../../../inode.md) and no useful [buffer cache](../../../../../../buffer-cache.md) entries for the three blocks; an uncached [inode](../../../../../../inode.md) adds one read. Under one-based byte numbering the last offset is 1567, without changing either address-block index or the read count.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
