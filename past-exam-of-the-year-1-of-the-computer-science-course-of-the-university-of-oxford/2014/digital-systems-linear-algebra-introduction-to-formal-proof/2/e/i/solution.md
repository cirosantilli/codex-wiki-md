<h1 id="2/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each address uses $32/8=4$ bytes, so an address block holds $q=2048/4=512$ pointers. Use zero-based [file offsets](../../../../../../file-offset.md). The requested [file offset](../../../../../../file-offset.md) has

$$
3000=1\cdot2048+952.
$$

Thus select direct pointer index 1, read its [file data block](../../../../../../file-data-block.md), and take the byte at offset 952 within it. No address block is needed:

$$
\boxed{1\text{ data-block read, assuming the inode is already resident}.}
$$

Fetching an uncached [inode](../../../../../../inode.md) adds one read. If “byte 3000” instead uses one-based numbering, the within-block offset is 951; it is still the second [file data block](../../../../../../file-data-block.md), with the same read count. Pathname lookup is separate from accessing a known [inode](../../../../../../inode.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
