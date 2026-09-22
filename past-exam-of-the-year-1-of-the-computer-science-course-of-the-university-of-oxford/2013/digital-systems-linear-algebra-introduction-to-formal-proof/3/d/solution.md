<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The predecessor [disk block number](../../../../../disk-block-number.md) turns the forward chain into a [doubly linked list](../../../../../doubly-linked-list.md). Starting from the header's last block, one can traverse backwards; removing or detaching the current block can find its predecessor directly rather than scanning from the beginning. When modifying a chain, the affected predecessor and successor links must both be updated consistently.

The file number identifies the owner of each [file data block](../../../../../file-data-block.md). A [file-system consistency checker](../../../../../file-system-consistency-checker.md) can scan the medium, group blocks by owner, detect a cross-link between different files, and help reconstruct chains or headers after damage. It also lets the system check that a block reached through a chain belongs to the expected file.

Thus

$$
\boxed{\text{predecessor: reverse traversal and editing; owner: validation and recovery}.}
$$

The extra metadata aids recovery but does not by itself guarantee [file-system crash consistency](../../../../../file-system-crash-consistency.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
