# Sv39 page table

↑ **Parent:** [Multi-level page table](multi-level-page-table.md)

The actual [Sv39 page table](sv39-page-table.md) geometry uses three nine-[bit](bit.md) indices and a twelve-[bit](bit.md) offset for base 4096-[byte](byte.md) [memory pages](memory-page.md). Each table contains 512 eight-[byte](byte.md) [page table entries](page-table-entry.md), exactly one 4096-[byte](byte.md) [memory page](memory-page.md); the `satp` [processor register](processor-register.md) identifies the root. A 64-[bit](bit.md) [virtual address](virtual-address.md) must repeat bit 38 in bits 63 through 39. Higher-level terminal entries can also map aligned larger [memory pages](memory-page.md), shortening the [page table walk](page-table-walk.md). These rules differ from the 16-[bit](bit.md), four-[byte](byte.md)-entry [two-level address translation](two-level-address-translation.md) model. [Version 20260120, section 12.4.1, printed pp. 136–137, Figures 68–70: address fields, entry sizes, root, and larger pages](the-risc-v-instruction-set-manual-volume-ii-privileged-architecture-by-risc-v-international.md)

For ordinary [Sv39 page tables](sv39-page-table.md), valid nonterminal [page table entries](page-table-entry.md) reference the next table with read, write, and execute flags clear; those clear flags do not prohibit reading the eventual data. The terminal entry supplies access permissions, with additional [processor privilege level](processor-privilege-level.md) and status checks. An invalid entry, malformed encoding, or denied access can cause a [page fault](page-fault.md). Thus the model's [set intersection](set-intersection.md) of read/write permissions at both levels must not be applied mechanically to [Sv39 page tables](sv39-page-table.md). [Version 20260120, section 12.3.2, printed p. 134, steps 2–8; section 12.4.1, printed p. 137: Sv39 uses the same algorithm with LEVELS=3 and PTESIZE=8](the-risc-v-instruction-set-manual-volume-ii-privileged-architecture-by-risc-v-international.md)

In [xv6 RISC-V source code](xv6-risc-v-source-code.md), root allocation is separate from lower-level allocation: `uvmcreate()` allocates and clears a root [page table](page-table.md), while `walk()` with allocation enabled allocates and clears missing lower-level tables and installs valid references to them. With allocation disabled, a missing table makes `walk()` return failure. This software routine finds a [page table entry](page-table-entry.md) for the [operating system](operating-system-split.md); it is not the hardware's complete permission-checking [page table walk](page-table-walk.md). [walk(): three-level index comment and alloc-controlled creation; uvmcreate(): root allocation and initialization](xv6-risc-v-source-code/vm-c.md)

## ↑ Ancestors (7)

1. [Multi-level page table](multi-level-page-table.md)
2. [Page table](page-table.md)
3. [Paging](paging.md)
4. [Virtual memory](virtual-memory-split.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Sv39 page table](sv39-page-table.md)
- [Two-level address translation](two-level-address-translation.md)
