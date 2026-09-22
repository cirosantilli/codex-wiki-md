# File-system consistency checker

↑ **Parent:** [File-system crash consistency](file-system-crash-consistency.md)

A program that compares independently represented facts in a [file system](file-system-split.md), such as the [hard link](hard-link.md) counts in [inodes](inode.md) versus references found in [directory entries](directory-entry.md), or the [block allocation bitmap](block-allocation-bitmap.md) versus block ownership recovered from [inodes](inode.md) and reserved structures. Disagreement detects corruption; repair policies must decide which evidence to trust and preserve recoverable data. A scan of names alone is insufficient to infer live ownership while the [file system](file-system-split.md) is changing or has unnamed open [files](computer-file.md), so checking requires a suitable stable view.

## ↑ Ancestors (6)

1. [File-system crash consistency](file-system-crash-consistency.md)
2. [File-system journaling](file-system-journaling.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/digital-systems-linear-algebra-introduction-to-formal-proof/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/d/solution.md)
