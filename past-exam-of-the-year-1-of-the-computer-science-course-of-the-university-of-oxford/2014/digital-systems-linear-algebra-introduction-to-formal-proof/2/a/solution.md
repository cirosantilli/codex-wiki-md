<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Names live in [directory entries](../../../../../directory-entry.md). Each ordinary [directory entry](../../../../../directory-entry.md) associates a component name with an [inode number](../../../../../inode-number.md); the corresponding [inode](../../../../../inode.md) describes the [file](../../../../../computer-file.md) and locates its contents. A name is therefore not stored as the identity of the [inode](../../../../../inode.md), and [hard links](../../../../../hard-link.md) can give one [inode](../../../../../inode.md) several names.

To resolve `/var/mail/user`, start from the root [file-system directory](../../../../../file-system-directory.md)'s [inode](../../../../../inode.md), read its [directory entries](../../../../../directory-entry.md) and find `var`. Follow that entry's [inode number](../../../../../inode-number.md) to the `var` [inode](../../../../../inode.md); read that [file-system directory](../../../../../file-system-directory.md) and find `mail`; repeat for `user`. The final [inode](../../../../../inode.md) supplies the [file metadata](../../../../../file-metadata.md) and addresses needed to read the [file data blocks](../../../../../file-data-block.md). The intermediate [file-system directories](../../../../../file-system-directory.md) require search permission. This describes ordinary pathname traversal without a [symbolic link](../../../../../symbolic-link.md) or mount point changing the route.

$$
\boxed{\text{component name}\longrightarrow\text{directory entry}\longrightarrow\text{inode}\longrightarrow\text{contents}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
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
