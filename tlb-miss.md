# TLB miss

↑ **Parent:** [Translation lookaside buffer](translation-lookaside-buffer.md)

A lookup that fails to find the required cached [address translation](address-translation.md). A successful refill can leave the [memory page](memory-page.md) resident throughout and cause no [page fault](page-fault.md).

For process A's resident virtual page 4 in [address translation](address-translation.md), discarding only its [translation lookaside buffer](translation-lookaside-buffer.md) entry makes the next read a [TLB miss](tlb-miss.md) while its contents remain in [page frame](page-frame.md) 13. [Page replacement](page-replacement.md) would instead remove the resident [memory page](memory-page.md); these operations invalidate different kinds of cached information.

## ↑ Ancestors (6)

1. [Translation lookaside buffer](translation-lookaside-buffer.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Memory management unit](memory-management-unit.md)
- [Page table walk](page-table-walk.md)
- [Sparse page table allocation](sparse-page-table-allocation.md)
- [TLB miss](tlb-miss.md)
- [Translation lookaside buffer](translation-lookaside-buffer.md)
- [Two-level address translation](two-level-address-translation.md)
