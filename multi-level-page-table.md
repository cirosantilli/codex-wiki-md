# Multi-level page table

↑ **Parent:** [Page table](page-table.md)

A hierarchy of [page tables](page-table.md) indexed by successive groups of virtual page number [bits](bit.md). Unused regions can omit lower-level tables.

The useful omission is an entire lower-level [array](array-data-structure.md), not merely an invalid [page table entry](page-table-entry.md). One absent upper-level entry can represent a large unmapped interval of the [address space](address-space.md). The [Linux kernel](linux-kernel.md)'s documented hierarchy uses this idea to avoid allocating tables for unused regions; its software levels can also be folded to match the hardware. [Page Tables: opening hierarchy discussion, paragraph beginning "One could of course imagine"; Page Table Folding](page-tables-by-the-kernel-development-community.md)

**Table of contents**

- [Two-level address translation](two-level-address-translation.md)
- [Sparse page table allocation](sparse-page-table-allocation.md)
- [Sv39 page table](sv39-page-table.md)

## ↑ Ancestors (6)

1. [Page table](page-table.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Page table](page-table.md)
- [Page table entry](page-table-entry.md)
