# Buffer cache key

↑ **Parent:** [Buffered device block](buffered-device-block.md)

The identity used to find a [buffered device block](buffered-device-block.md). In the fixed-block-size model, $d$ identifies the device and $b$ its block number; $(d_1,7)$ and $(d_2,7)$ are different keys if $d_1\ne d_2$. A [file](computer-file.md)'s pathname or its logical block offset alone is insufficient for this device-indexed model. Interfaces supporting different transfer sizes need to specify the size and overlap rules too.

Maintain at most one logical [buffered device block](buffered-device-block.md) for each [buffer cache key](buffer-cache-key.md) within this [buffer cache](buffer-cache.md). Otherwise two callers could modify different copies and later overwrite one another's changes. Lookup and reservation must therefore be coordinated by [synchronization](synchronization-computing.md): even before contents are ready, a reserved key directs a second caller to the same structure. This invariant concerns the participating cache, not every copy of those [bytes](byte.md) anywhere in the machine.

## ↑ Ancestors (6)

1. [Buffered device block](buffered-device-block.md)
2. [Buffer cache](buffer-cache.md)
3. [File system](file-system.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Buffer cache key](buffer-cache-key.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Buffer cache validity](buffer-cache-validity.md)
- [Buffered device block](buffered-device-block.md)
- [Dirty buffer](dirty-buffer.md)
- [Page cache](page-cache.md)
