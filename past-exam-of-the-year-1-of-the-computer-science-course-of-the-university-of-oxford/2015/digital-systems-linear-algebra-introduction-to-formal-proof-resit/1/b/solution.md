<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [file-system namespace](../../../../../file-system-namespace.md) is rooted at the root [file-system directory](../../../../../file-system-directory.md). Each [directory entry](../../../../../directory-entry.md) associates a local name with an [inode number](../../../../../inode-number.md). To resolve a pathname, start at the root for an absolute pathname, or at the process's current [file-system directory](../../../../../file-system-directory.md) for a relative pathname, and look up successive components in successive [file-system directories](../../../../../file-system-directory.md). A [file-system directory](../../../../../file-system-directory.md) is itself a [file](../../../../../computer-file.md) with a special interpretation for its data.

The [inode table](../../../../../inode-table.md) stores [file metadata](../../../../../file-metadata.md) and the information locating contents. The [file-system directory](../../../../../file-system-directory.md) structure supplies names and the connections used in pathname lookup. Thus the [file](../../../../../computer-file.md) is the object represented by its [inode](../../../../../inode.md), whereas a file name is one entry referring to that object. Two [hard links](../../../../../hard-link.md) can give the same [file](../../../../../computer-file.md) two names, possibly in different [file-system directories](../../../../../file-system-directory.md). Renaming a [file](../../../../../computer-file.md) need not move its contents or change its [inode number](../../../../../inode-number.md); after [unlinking an open file](../../../../../unlinking-an-open-file.md), a [file](../../../../../computer-file.md) can temporarily have no names and still be accessible through an existing [file descriptor](../../../../../file-descriptor.md).

$$
\boxed{\text{names locate inodes; inodes describe files and locate contents.}}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
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
