<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A traditional [inode](../../../../../inode.md) uses a fixed number of direct pointers to [file data blocks](../../../../../file-data-block.md), followed by singly, doubly and sometimes triply [indirect block pointers](../../../../../indirect-block-pointer.md). A singly [indirect block pointer](../../../../../indirect-block-pointer.md) reaches one address block whose entries point to [file data blocks](../../../../../file-data-block.md). A doubly [indirect block pointer](../../../../../indirect-block-pointer.md) reaches a block of pointers to singly indirect address blocks; a triply indirect one adds another level. The [file data blocks](../../../../../file-data-block.md) need not be physically contiguous.

This [multilevel inode indexing](../../../../../multilevel-inode-indexing.md) keeps the [inode](../../../../../inode.md) compact. A small [file](../../../../../computer-file.md) uses direct pointers without allocating address blocks, while a large [file](../../../../../computer-file.md) allocates deeper address blocks only as needed. If each address block holds $q$ addresses, the successive levels cover $q,q^2,q^3$ [file data blocks](../../../../../file-data-block.md). The logical [file offset](../../../../../file-offset.md) selects a path arithmetically, so random access does not require walking through all preceding [file data blocks](../../../../../file-data-block.md).

$$
\boxed{\text{small files: direct access; large files: additional indirection levels}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
