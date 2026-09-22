<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Reserve a large sparse region of the 64-bit [virtual memory](../../../../../../virtual-memory.md) space for each open file, returning its base address or a segment handle. Access byte $j$ through the address base plus $j$. Choose nonoverlapping page-aligned reservations, retain a file-identifier/offset/length mapping descriptor and apply file access rights as memory permissions. A conceptual division into high-order file-slot bits and low-order offset bits is possible, but the split is a design choice and must leave adequate maximum file size and slot count.

Use sparse multilevel [page tables](../../../../../../page-table.md): reserving an address interval must not allocate physical storage or a dense table for every possible byte. A first access produces a [page fault](../../../../../../page-fault.md), locates the corresponding file page in the filesystem/page cache, reads it if absent, installs a mapping and restarts the instruction. Several processes mapping the same file page can share the same physical frame, maintaining one coherent cached copy. Read-only mappings forbid stores; writable mappings mark dirty pages for eventual writeback, with an explicit synchronization operation when durability is required.

Opening and mapping records the virtual reservation; closing or unmapping removes it and performs required writeback. Extension may enlarge the mapping and file according to the API, while access beyond the logical end or after truncation must be checked and reported rather than silently exposing another object. The spare bytes of the last page need an explicit convention, since page-granularity hardware alone cannot enforce every byte-level file limit. Sharing, concurrent edits and stale handles require suitable locking, mapping invalidation and lifecycle rules. **Demand-paged [memory-mapped files](../../../../../../memory-mapped-file.md) realize the [Multics](../../../../../../multics.md) view without reading entire files or allocating their whole address reservations in RAM.** A nominal 64-bit address type does not guarantee that every hardware implementation exposes all $2^{64}$ addresses, so reservations use the supported range.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
