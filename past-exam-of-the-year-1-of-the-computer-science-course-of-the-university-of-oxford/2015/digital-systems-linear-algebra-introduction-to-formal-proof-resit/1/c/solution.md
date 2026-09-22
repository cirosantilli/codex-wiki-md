<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [block allocation bitmap](../../../../../block-allocation-bitmap.md), one [bit](../../../../../bit.md) per allocatable [disk block number](../../../../../disk-block-number.md), or a [free-block list](../../../../../free-block-list.md). Allocation removes a free block from the free representation; deallocation inserts it. Reserved [file system](../../../../../file-system-split.md) structures, including the [inode table](../../../../../inode-table.md) and the free-space representation itself, must never be offered as free [file data blocks](../../../../../file-data-block.md). Free [inodes](../../../../../inode.md) can be tracked separately by an [inode allocation bitmap](../../../../../inode-allocation-bitmap.md).

A [file data block](../../../../../file-data-block.md) becomes reusable when the [file system](../../../../../file-system-split.md) has removed its ownership from the [file](../../../../../computer-file.md). This happens, for example, when truncation discards that portion of the [file](../../../../../computer-file.md), or when the [file](../../../../../computer-file.md) is finally destroyed. Destruction requires both removal of its last [hard link](../../../../../hard-link.md) and release of its last live reference: [unlinking an open file](../../../../../unlinking-an-open-file.md) must not reclaim blocks still needed through an [open file description](../../../../../open-file-description.md). A [memory-mapped file](../../../../../memory-mapped-file.md), if supported, also requires its references to be accounted for. The [indirect block pointers](../../../../../indirect-block-pointer.md)' own blocks are reclaimed when they are no longer needed.

There are two relevant notions of accessibility. Pathname-accessible [files](../../../../../computer-file.md) are those reached from the root through valid [directory entries](../../../../../directory-entry.md), subject to permissions; their allocated blocks are found through their [inodes](../../../../../inode.md). Already-open [files](../../../../../computer-file.md) can additionally remain accessible through [file descriptors](../../../../../file-descriptor.md) even after their last names disappear. Allocated [file system](../../../../../file-system-split.md) structures and blocks pinned by an operation must also be excluded from allocation. A [block allocation bitmap](../../../../../block-allocation-bitmap.md) must therefore describe actual allocation, rather than merely the blocks of currently named regular [files](../../../../../computer-file.md).

One processor can still run several processes and be interrupted. Updating ownership and the free-space representation must therefore be serialized with respect to competing operations, for example through an appropriate kernel critical section. Persistence across a crash additionally requires [file-system crash consistency](../../../../../file-system-crash-consistency.md), such as ordered updates or [file-system journaling](../../../../../file-system-journaling.md).

$$
\boxed{\text{last name removed}\ \not\Rightarrow\ \text{open-file blocks immediately free}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
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
