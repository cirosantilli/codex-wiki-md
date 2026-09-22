<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the traditional [Unix](../../../../../unix.md) [file system](../../../../../file-system-split.md) model, a regular [file](../../../../../computer-file.md) consists of [file metadata](../../../../../file-metadata.md) in an [inode](../../../../../inode.md) and an ordered sequence of [bytes](../../../../../byte.md) stored in [file data blocks](../../../../../file-data-block.md). The [inode](../../../../../inode.md) records the type, owner, permissions, length, timestamps and [hard link](../../../../../hard-link.md) count, together with the information locating its [file data blocks](../../../../../file-data-block.md). A small [file](../../../../../computer-file.md) can use direct [file data block](../../../../../file-data-block.md) addresses; a larger [file](../../../../../computer-file.md) can additionally use [indirect block pointers](../../../../../indirect-block-pointer.md), whose blocks contain further addresses rather than user data. The final [file data block](../../../../../file-data-block.md) need not be completely occupied.

An [inode number](../../../../../inode-number.md) identifies an entry in the [inode table](../../../../../inode-table.md) of this [file system](../../../../../file-system-split.md); it identifies the [file](../../../../../computer-file.md), rather than a particular piece of its contents. A [disk block number](../../../../../disk-block-number.md) identifies a fixed-size storage region on the volume. Resolving an [inode number](../../../../../inode-number.md) first obtains the [inode](../../../../../inode.md); following its direct or [indirect block pointers](../../../../../indirect-block-pointer.md) then finds the required [file data block](../../../../../file-data-block.md). The two numbers belong to different address spaces, even though the [inode table](../../../../../inode-table.md) itself occupies disk blocks.

$$
\boxed{\text{inode number: file identity; block number: storage location.}}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
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
