# Multilevel inode indexing

↑ **Parent:** [Indirect block pointer](indirect-block-pointer.md)

An [inode](inode.md)-based [file system](file-system-split.md) uses direct pointers for small [files](computer-file.md) and successive levels of [indirect block pointers](indirect-block-pointer.md) for larger ones. If an address block contains $q$ pointers, a depth-$k$ region addresses $q^k$ [file data blocks](file-data-block.md). With the [inode](inode.md) resident, an uncached byte access in that region requires $k$ address-block reads and one [file data block](file-data-block.md) read.

## ↑ Ancestors (6)

1. [Indirect block pointer](indirect-block-pointer.md)
2. [Inode](inode.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/2/f/solution.md)
