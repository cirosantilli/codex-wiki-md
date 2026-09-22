# Dirty memory page

↑ **Parent:** [Page replacement](page-replacement.md)

A resident [memory page](memory-page.md) with modifications that must be preserved in its backing storage before its [page frame](page-frame.md) can be reused. In the simple model here, a write sets its dirty flag, and successful [page writeback](page-writeback.md) clears it. A clean [memory page](memory-page.md) with a recoverable backing copy can be discarded without an outgoing data write.[Section 22.9, p. 13: modified/dirty bit and the outgoing I/O difference between dirty and clean eviction](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

**Table of contents**

- [Page writeback](page-writeback.md)

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Page-reference trace](page-reference-trace.md)
- [Page replacement](page-replacement.md)
- [Page-replacement cost accounting](page-replacement-cost-accounting.md)
- [Page writeback](page-writeback.md)
- [Shared file mapping](shared-file-mapping.md)
