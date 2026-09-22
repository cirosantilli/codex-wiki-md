# CLOCK page replacement

↑ **Parent:** [Page replacement](page-replacement.md)

Keep frames in a circular list with a reference flag and a scanning hand. Clear set flags while scanning; choose the first eligible frame with a clear flag. This second chance approximates [LRU replacement](lru-replacement.md) with cheaper tracking. When hardware reference flags are absent, revoking a mapping and handling its first later [page fault](page-fault.md) can supply a software reference observation.

// Destination: computer-science.bigb

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/c/solution.md)
