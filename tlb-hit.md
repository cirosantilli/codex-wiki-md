# TLB hit

↑ **Parent:** [Translation lookaside buffer](translation-lookaside-buffer.md)

A lookup that finds a valid cached [address translation](address-translation.md) for the relevant [address space](address-space.md). The access can still cause a [page fault](page-fault.md) if the cached permissions forbid it.

For the 64-[byte](byte.md) toy model in [address translation](address-translation.md), a cached process A page-4 mapping covers reads at both `0x12D` and `0x12E`, yielding [physical addresses](physical-address.md) `0x36D` and `0x36E`. The [TLB hit](tlb-hit.md) reuses the mapping; it does not guarantee that either requested [byte](byte.md) is in a data [memory cache](cache-computing.md).

## ↑ Ancestors (6)

1. [Translation lookaside buffer](translation-lookaside-buffer.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Memory management unit](memory-management-unit.md)
- [TLB hit](tlb-hit.md)
- [Translation lookaside buffer](translation-lookaside-buffer.md)
- [Two-level address translation](two-level-address-translation.md)
