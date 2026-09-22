# Page table

↑ **Parent:** [Paging](paging.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Page_table)

A [page table](page-table.md) is the [data structure](data-structure-split.md) describing an [address space](address-space.md)'s mappings from virtual page numbers to [page frames](page-frame.md), together with access and status information. A [page table entry](page-table-entry.md) can describe a resident [memory page](memory-page.md) and its permissions. Nonresident or unmapped [memory pages](memory-page.md) require a representation that lets the [operating system](operating-system-split.md) distinguish them; a hardware not-present flag alone need not make that distinction. On [x86](x86.md), additional [operating system](operating-system-split.md) information determines whether a not-present mapping is legitimate. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 18, section 18.3: page-table contents and the x86 present bit](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-paging.pdf)

The four rows drawn under [paging](paging.md) are an illustrative model, combining [page table](page-table.md) and [operating system](operating-system-split.md) information: virtual page `0x12` is resident in physical frame `0x07` with read-only permission; `0x13` is resident in `0x02` with read/write permission; `0x14` is mapped read/write but nonresident; `0x15` is unmapped. The labels deliberately separate mapping policy, residency and permission. They are not a literal [x86](x86.md) entry layout. A [translation lookaside buffer](translation-lookaside-buffer.md) valid flag is a fourth, independent notion: it says that a cached translation can be considered, not that every resident [memory page](memory-page.md) has a cached translation.

A flat [array](array-data-structure.md) with one [page table entry](page-table-entry.md) per virtual page would have $2^{16}/256=256$ entries in this example. At an assumed four [bytes](byte.md) per entry, it occupies $256\cdot4=1024$ [bytes](byte.md), whether one [memory page](memory-page.md) or all 256 [memory pages](memory-page.md) are mapped. A [multi-level page table](multi-level-page-table.md) saves space in sparse [address spaces](address-space.md) by allocating lower-level tables only for the regions that need them. The tradeoff is extra dependent lookups during a [page table walk](page-table-walk.md); a [translation lookaside buffer](translation-lookaside-buffer.md) avoids repeating those lookups on a hit. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 20: Paging, Smaller Tables, section 20.3](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-smalltables.pdf)

**Table of contents**

- [Page table entry](page-table-entry.md)
- [Multi-level page table](multi-level-page-table.md)
  - [Two-level address translation](two-level-address-translation.md)
  - [Sparse page table allocation](sparse-page-table-allocation.md)
  - [Sv39 page table](sv39-page-table.md)
- [Page table walk](page-table-walk.md)

## ↑ Ancestors (5)

1. [Paging](paging.md)
2. [Virtual memory](virtual-memory-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Context switch](context-switch.md)
- [Copy-on-write](copy-on-write.md)
- [Copy-on-write fault handling](copy-on-write-fault-handling.md)
- [Copy-on-write page accounting](copy-on-write-page-accounting.md)
- [Memory management unit](memory-management-unit.md)
- [Memory-mapped file](memory-mapped-file.md)
- [Memory-mapped file offset translation](memory-mapped-file-offset-translation.md)
- [Multi-level page table](multi-level-page-table.md)
- [Page fault](page-fault.md)
- [Page table](page-table.md)
- [Page table entry](page-table-entry.md)
- [Paging](paging.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/d/solution.md)
- [Sv39 page table](sv39-page-table.md)
- [Two-level address translation](two-level-address-translation.md)
- [Virtual memory](virtual-memory-split.md)
