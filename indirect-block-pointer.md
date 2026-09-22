# Indirect block pointer

↑ **Parent:** [Inode](inode.md)

An address in a traditional [inode](inode.md)-based [file system](file-system-split.md) that points to a block of further [disk block numbers](disk-block-number.md), rather than directly to user contents. If a block can store $q$ addresses, one singly indirect block can locate up to $q$ [file data blocks](file-data-block.md), and a doubly indirect arrangement can locate up to $q^2$. The address blocks themselves consume allocated storage and must be reclaimed when their [file](computer-file.md) no longer needs them. This lets small [files](computer-file.md) use a short direct layout while supporting larger [files](computer-file.md).

**Table of contents**

- [Multilevel inode indexing](multilevel-inode-indexing.md)

## ↑ Ancestors (5)

1. [Inode](inode.md)
2. [File system](file-system-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Multilevel inode indexing](multilevel-inode-indexing.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/digital-systems-linear-algebra-introduction-to-formal-proof/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/2/e/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/d/solution.md)
