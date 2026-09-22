# Copy-on-write fault handling

↑ **Parent:** [Copy-on-write](copy-on-write.md)

The [operating-system kernel](kernel-operating-system.md) must distinguish a temporarily protected [copy-on-write](copy-on-write.md) mapping from one whose writes are forbidden. The teaching procedure in MIT's xv6 lab protects both [page tables](page-table.md), copies the shared [page frame](page-frame.md) on a valid write [page fault](page-fault.md), and installs a writable [page table entry](page-table-entry.md). Originally read-only code remains read-only. Its [reference counting](reference-counting.md) increments on sharing and decrements on removal; storage is freed only after the last reference disappears. The lab also requires kernel writes into user storage to respect [copy-on-write](copy-on-write.md), and specifies failure if no free storage remains. [Lab: Copy-on-Write Fork for xv6](6-1810-and-fall-2022/lab-copy-on-write-fork-for-xv6.md)

Every write must respect the sharing policy, but every write need not copy. Repeated writes to B's already private writable F3 need no further [copy-on-write](copy-on-write.md) [page fault](page-fault.md). If A later writes F0, an implementation can reuse F0 when it establishes exclusive, writable ownership; A's remaining read-only [page table entry](page-table-entry.md) may still need a [page fault](page-fault.md) to enable the write. This exclusive-reuse rule is an assumption of [copy-on-write page accounting](copy-on-write-page-accounting.md) below, not a promise that every [operating system](operating-system-split.md) uses that path. A count of one alone is not a universal permission to alter storage belonging to a [memory-mapped file](memory-mapped-file.md) or another owner.

Changing mappings or permissions must also make cached [address translations](address-translation.md) consistent. [Cache and TLB Flushing Under Linux by David S. Miller](cache-and-tlb-flushing-under-linux-by-david-s-miller.md) Concurrent [software threads](thread-computing.md) require [synchronization](synchronization-computing.md) around ownership checks, copying, and installation to prevent a [race condition](race-condition.md); neither diagrams nor counts specify a production [operating-system kernel](kernel-operating-system.md)'s locking or hardware invalidation protocol.

## ↑ Ancestors (5)

1. [Copy-on-write](copy-on-write.md)
2. [Virtual memory](virtual-memory-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Copy-on-write](copy-on-write.md)
- [Memory protection](memory-protection.md)
