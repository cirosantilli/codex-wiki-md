<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [file descriptor table](../../../../../file-descriptor-table.md) belongs to a process: its small nonnegative [integer](../../../../../integer-split.md) indices are [file descriptors](../../../../../file-descriptor.md), and each occupied entry points to an [open file description](../../../../../open-file-description.md). It also holds descriptor-specific information, such as whether the descriptor closes on a successful program replacement. There is **one logical [file descriptor table](../../../../../file-descriptor-table.md) per process** in the traditional model; implementations can let processes explicitly share one.

The system-wide [open file table](../../../../../open-file-table.md), called the file pointer table here, contains [open file descriptions](../../../../../open-file-description.md). Each entry records an opening's access mode, current [file offset](../../../../../file-offset.md), reference count and reference to an in-memory [inode](../../../../../inode.md). Duplicated [file descriptors](../../../../../file-descriptor.md), including inherited ones, can refer to the same [open file description](../../../../../open-file-description.md) and therefore share its [file offset](../../../../../file-offset.md). Independent opens of the same [file](../../../../../computer-file.md) normally create separate [open file descriptions](../../../../../open-file-description.md) and separate offsets. There is **one logical system-wide [open file table](../../../../../open-file-table.md)**, with many entries.

The system-wide in-memory [inode table](../../../../../inode-table.md) caches the [inodes](../../../../../inode.md) currently needed, including shared [file metadata](../../../../../file-metadata.md), locking and reference information. Its identity key must include the [file system](../../../../../file-system-split.md) as well as the [inode number](../../../../../inode-number.md) when several volumes are mounted. There is **one logical system-wide active [inode table](../../../../../inode-table.md)**, distinct from the persistent [inode table](../../../../../inode-table.md) stored on each volume. These are logical organizations, not requirements for a single contiguous array in memory.

$$
\boxed{\text{process descriptor}\to\text{open-file description}\to\text{active inode}\to\text{disk blocks}.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
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
