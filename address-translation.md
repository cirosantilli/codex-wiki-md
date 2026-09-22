# Address translation

↑ **Parent:** [Virtual memory](virtual-memory-split.md)

Converting a [virtual address](virtual-address.md) to a [physical address](physical-address.md) using the current [address space](address-space.md)'s mapping, with access checks. In [paging](paging.md), the [memory page](memory-page.md) number changes while the offset within it stays fixed.

[Address translation](address-translation.md) answers where an access would go; [memory protection](memory-protection.md) answers whether that access may proceed. Neither answer is the stored value. Reading the requested [bytes](byte.md) is a subsequent logical operation, served by a [memory cache](cache-computing.md) or main [computer memory](computer-memory.md). The [operating system](operating-system-split.md) establishes the mapping context used by the [memory management unit](memory-management-unit.md).[Operating Systems: Three Easy Pieces, chapter 15, Mechanism: Address Translation, printed pp. 1–2: hardware mechanism and operating-system control](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/mechanism-address-translation.md)

Consider an original toy model with unsigned 12-[bit](bit.md) [virtual addresses](virtual-address.md), [byte](byte.md) addressing, and 64-[byte](byte.md) [memory pages](memory-page.md) and [page frames](page-frame.md). Assume single-[byte](byte.md) reads, one [memory page](memory-page.md) size, no concurrent mapping changes, and resident readable mappings for virtual page 4 in both [address spaces](address-space.md). The [virtual address](virtual-address.md) $v=\mathtt{0x12D}=301$ has six page-number [bits](bit.md) and six offset [bits](bit.md), rather than a split between [hexadecimal](hexadecimal.md) digits. By [Euclidean division](euclidean-division.md),

$$
301=4\cdot64+45,\qquad q=4,\qquad d=45=\mathtt{0x2D}.
$$

Process A maps virtual page 4 to [page frame](page-frame.md) 13; process B maps it to [page frame](page-frame.md) 9. Thus the identical [virtual address](virtual-address.md) denotes

$$
a_A=13\cdot64+45=877=\mathtt{0x36D},\qquad a_B=9\cdot64+45=621=\mathtt{0x26D}.
$$

These are addresses, not the [bytes](byte.md) read there. If the example's contents at those [physical addresses](physical-address.md) are respectively 7 and 99, the two reads return 7 and 99. The mapping calculation alone cannot determine either value.

A [translation lookaside buffer](translation-lookaside-buffer.md) can cache these mappings and permissions. In a tagged version of this model, its lookup key includes the [address space identifier](address-space-identifier.md) as well as virtual page 4. An untagged version must remove conflicting cached mappings when changing the [address space](address-space.md). Which tags and invalidation operations are available depends on the architecture; a [context switch](context-switch.md) need not universally clear the whole [translation lookaside buffer](translation-lookaside-buffer.md).[Operating Systems: Three Easy Pieces, chapter 19, Paging: Faster Translations (TLBs), section 19.5, printed pp. 9–10: flushing and address-space identifiers](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/paging-faster-translations-tlbs.md)

The arithmetic explains the beauty of [paging](paging.md): a mapping can move an entire [memory page](memory-page.md) without changing its internal positions. Indeed, for two offsets $d_1,d_2$ in the same mapped [memory page](memory-page.md),

$$
(fP+d_2)-(fP+d_1)=d_2-d_1.
$$

For process A, virtual page 4 spans `0x100`–`0x13F` and maps to `0x340`–`0x37F`. Crossing from `0x13F` to `0x140` selects virtual page 5 and requires its own mapping and [memory protection](memory-protection.md) checks. A multi-[byte](byte.md) access crossing that boundary cannot be justified by checking only its first [byte](byte.md).

## ↑ Ancestors (4)

1. [Virtual memory](virtual-memory-split.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Address space identifier](address-space-identifier.md)
- [Address translation](address-translation.md)
- [Cache (computing)](cache-computing.md)
- [Copy-on-write fault handling](copy-on-write-fault-handling.md)
- [Memory management unit](memory-management-unit.md)
- [Memory-mapped file](memory-mapped-file.md)
- [Microkernel service failure isolation](microkernel-service-failure-isolation.md)
- [Physical address](physical-address.md)
- [TLB hit](tlb-hit.md)
- [TLB miss](tlb-miss.md)
- [Virtual address](virtual-address.md)
