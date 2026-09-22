# Page fault

↑ **Parent:** [Paging](paging.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Page_fault)

A [page fault](page-fault.md) transfers control to the [operating system](operating-system.md) when an access cannot proceed under the current [paging](paging.md) translation or protection rules. The term includes both unavailable translations and forbidden accesses on [x86](x86.md). Intel's manual distinguishes these causes; AMD's error code likewise distinguishes ordinary not-present faults from protection violations. Other architectural causes, including malformed [page table entries](page-table-entry.md), also exist. [Intel SDM, volume 3A, section 4.7: Page-Fault Exceptions](https://cdrdv2-public.intel.com/671200/325462-sdm-vol-1-2abcd-3abcd.pdf)[AMD64 Architecture Programmer's Manual, volume 2, revision 3.44, section 8.4.2: Page-Fault Error Code](https://docs.amd.com/api/khub/documents/sD1_QL~h4Afq2_tvzxqqSQ/content)

The illustrative [page table](page-table.md) in [paging](paging.md) separates three situations:
- A read at [virtual address](virtual-address.md) `0x1434` targets a permitted but nonresident [memory page](memory-page.md). The [operating system](operating-system.md) may supply it and retry the access.
- A write at [virtual address](virtual-address.md) `0x1234` targets a resident, read-only [memory page](memory-page.md). The [page fault](page-fault.md) is caused by missing write permission, not by missing contents.
- A read at [virtual address](virtual-address.md) `0x1534` targets an unmapped part of the [address space](address-space.md). The [operating system](operating-system.md) must reject it unless its policy authorizes creating a mapping.

A [page fault](page-fault.md) is not necessarily a program error or a storage-device read. [Demand paging](demand-paging.md) can allocate a zero-filled [page frame](page-frame.md) without reading secondary storage. A [copy-on-write](copy-on-write.md) write deliberately encounters read-only permissions; the [operating system](operating-system.md) supplies a private copy and enables the write. A truly forbidden access may instead terminate the [operating-system process](process-computing.md). The handler interprets the fault using both architectural fault information and its own mapping policy. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 23: demand zeroing and copy-on-write](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-complete.pdf)

For a nonresident [memory page](memory-page.md) whose contents must be loaded, the handler obtains a [page frame](page-frame.md), possibly invokes [page replacement](page-replacement.md), supplies the contents, updates the [page table](page-table.md), arranges any necessary [translation lookaside buffer](translation-lookaside-buffer.md) invalidation, and resumes the operation. If no mapping or permission can legally be supplied, it reports failure. This mechanism lets ordinary accesses request work only when it becomes necessary. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 21: Beyond Physical Memory, Mechanisms, sections 21.3–21.5](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-beyondphys.pdf)

// Target: computer-science.bigb

**Table of contents**

- [Page fault rate](page-fault-rate.md)

## ↑ Ancestors (5)

1. [Paging](paging.md)
2. [Virtual memory](virtual-memory.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (25)

- [CLOCK page replacement](clock-page-replacement.md)
- [Copy-on-write](copy-on-write.md)
- [Copy-on-write fault handling](copy-on-write-fault-handling.md)
- [Copy-on-write page accounting](copy-on-write-page-accounting.md)
- [Demand paging](demand-paging.md)
- [Interrupt](interrupt.md)
- [Memory-mapped file](memory-mapped-file.md)
- [Page fault](page-fault.md)
- [Page fault rate](page-fault-rate.md)
- [Page-reference trace](page-reference-trace.md)
- [Page replacement](page-replacement.md)
- [Page-replacement cost accounting](page-replacement-cost-accounting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/7/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/7/d/solution.md)
- [Private file mapping](private-file-mapping.md)
- [Sv39 page table](sv39-page-table.md)
- [Synchronous processor exception](synchronous-processor-exception.md)
- [Thrashing (computer science)](thrashing-computer-science.md)
- [TLB hit](tlb-hit.md)
- [TLB miss](tlb-miss.md)
- [Translation lookaside buffer](translation-lookaside-buffer.md)
- [Two-level address translation](two-level-address-translation.md)
