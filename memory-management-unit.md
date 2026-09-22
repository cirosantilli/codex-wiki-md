# Memory management unit

↑ **Parent:** [Virtual memory](virtual-memory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memory_management_unit)

The hardware that performs [address translation](address-translation.md) and access checks. Whether a [TLB miss](tlb-miss.md) is resolved entirely by hardware or with [operating system](operating-system-split.md) assistance depends on the architecture.

For [paging](paging.md), the [memory management unit](memory-management-unit.md) uses the active [address space](address-space.md) and the kind of access: reading, writing, or fetching an instruction. [Processor privilege level](processor-privilege-level.md) can also affect permission. A [TLB hit](tlb-hit.md) supplies cached translation attributes; it does not bypass [memory protection](memory-protection.md). On a [TLB miss](tlb-miss.md), some architectures perform a hardware [page table walk](page-table-walk.md), while others enter an [operating system](operating-system-split.md) refill handler. Both can resolve a resident mapping without a nonresident [page fault](page-fault.md).[Operating Systems: Three Easy Pieces, chapter 19, Paging: Faster Translations (TLBs), sections 19.1, 19.3–19.4, printed pp. 2, 6, 8: permission checks, refill ownership, and cached attributes](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/paging-faster-translations-tlbs.md)

<a id="image-logical-address-translation-control-path-a-cached-mapping-refill-permission-check-and-separate-data-read"></a>
![](address-translation-tlb-control-path.png)

**[Figure 1](#image-logical-address-translation-control-path-a-cached-mapping-refill-permission-check-and-separate-data-read). Logical address translation control path: a cached mapping, refill, permission check, and separate data read**.

This diagram is a logical dependency model for the toy single-[byte](byte.md) read, rather than a timing diagram for a particular [CPU](central-processing-unit.md). A [translation lookaside buffer](translation-lookaside-buffer.md) caches translations and access attributes; a data [memory cache](cache-computing.md) caches contents. A [TLB hit](tlb-hit.md) can accompany a data [cache miss](cache-miss.md), and a [TLB miss](tlb-miss.md) can accompany a data [cache hit](cache-hit.md) after successful refill. Reading [page table entries](page-table-entry.md) during refill is also distinct from reading the requested data. Actual implementations may overlap steps.

Extend process A's toy [address space](address-space.md) with these independent starting states. Virtual page 4 is resident in [page frame](page-frame.md) 13 and readable but not writable. Virtual page 5 is a permitted readable [memory page](memory-page.md) whose old contents are in backing storage and which is initially nonresident. Virtual page 6 has no mapping authorized by the [operating system](operating-system-split.md). Assume permission changes and eviction always invalidate affected cached translations before later accesses, no [copy-on-write](copy-on-write.md) policy, and a free [page frame](page-frame.md) 2 for loading virtual page 5.

- Read `0x12D` with an empty [translation lookaside buffer](translation-lookaside-buffer.md): a [TLB miss](tlb-miss.md) discovers resident virtual page 4, caches its attributes, and reads [physical address](physical-address.md) `0x36D`. There is no nonresident [page fault](page-fault.md).
- Write `0x12D` with that translation already cached: a [TLB hit](tlb-hit.md) finds the mapping, but [memory protection](memory-protection.md) denies the write. The target [byte](byte.md) remains unchanged even though its [page frame](page-frame.md) is resident.
- Read `0x16D`: virtual page 5 and offset 45 are permitted but nonresident. A [page fault](page-fault.md) lets the [operating system](operating-system-split.md) load the contents into [page frame](page-frame.md) 2, update the [page table](page-table.md), and retry. Successful [address translation](address-translation.md) then gives $2\cdot64+45=173=\mathtt{0x0AD}$; the requested read occurs only after the contents are ready.
- Read `0x1AD`: virtual page 6 and offset 45 have no authorized mapping. The [operating system](operating-system-split.md) rejects the access in this model; finding a free [page frame](page-frame.md) would not supply authorization.

<a id="image-four-original-access-traces-distinguish-tlb-misses-denied-writes-nonresident-memory-pages-and-unauthorized-addresses"></a>
![](memory-access-permission-residency-traces.png)

**[Figure 2](#image-four-original-access-traces-distinguish-tlb-misses-denied-writes-nonresident-memory-pages-and-unauthorized-addresses). Four original access traces distinguish TLB misses, denied writes, nonresident memory pages, and unauthorized addresses**.

A nonresident [memory page](memory-page.md) and a forbidden access therefore require different decisions: supplying contents can repair the former, while the latter needs authorization. Fault terminology and the encoding of [page table entries](page-table-entry.md) vary by architecture; the model's distinct states do not assert distinct hardware exception names or a universal order of checks.[Operating Systems: Three Easy Pieces, chapter 21, Beyond Physical Memory: Mechanisms, sections 21.2–21.5, printed pp. 3–7, especially the terminology aside and Figures 21.2–21.3](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-mechanisms.md)

The separation makes [virtual memory](virtual-memory-split.md) useful: ordinary accesses can reuse cached mappings while the [operating system](operating-system-split.md) intervenes when policy or residency requires work. It also makes failures easier to diagnose. A lost cached translation, unavailable contents, and denied permission are three different obstacles, even when all interrupt the same requested read.

## ↑ Ancestors (4)

1. [Virtual memory](virtual-memory-split.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Address translation](address-translation.md)
- [Context switch](context-switch.md)
- [Direct memory access](direct-memory-access.md)
- [Memory management unit](memory-management-unit.md)
- [Memory protection](memory-protection.md)
- [Virtual memory](virtual-memory-split.md)
