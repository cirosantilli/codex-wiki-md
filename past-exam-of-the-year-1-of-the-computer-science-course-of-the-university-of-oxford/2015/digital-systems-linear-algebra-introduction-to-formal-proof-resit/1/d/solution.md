<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [hard link](../../../../../hard-link.md) count in an [inode](../../../../../inode.md) duplicates information recoverable by counting [directory entries](../../../../../directory-entry.md) that refer to its [inode number](../../../../../inode-number.md). Keeping the count makes the last-name test fast: a [hard link](../../../../../hard-link.md) removal need not search every [file-system directory](../../../../../file-system-directory.md). A [file-system consistency checker](../../../../../file-system-consistency-checker.md) can independently recount the references and compare the result with the stored value.

Likewise, a [block allocation bitmap](../../../../../block-allocation-bitmap.md) summarizes ownership information recoverable from allocated [inodes](../../../../../inode.md), their [file data blocks](../../../../../file-data-block.md), their [indirect block pointers](../../../../../indirect-block-pointer.md), and reserved [file system](../../../../../file-system-split.md) structures. This summary makes allocation efficient and supplies an independent consistency check against multiply allocated or lost blocks. Replicated superblock information is another possible form of [data redundancy](../../../../../data-redundancy.md), helping recovery if one copy is damaged. These examples have distinct benefits: a cached count or allocation summary saves work, while an independent or replicated representation helps detect or repair corruption. Consistent updating is essential; redundancy alone does not make a [file system](../../../../../file-system-split.md) crash-safe.

$$
\boxed{\text{redundancy supports efficient lookup, consistency checking and recovery.}}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
