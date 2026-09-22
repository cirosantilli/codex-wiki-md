# Dirty buffer

↑ **Parent:** [Buffered device block](buffered-device-block.md)

A valid [buffered device block](buffered-device-block.md) with modifications still owed to its backing location. Until successful [buffer cache writeback](buffer-cache-writeback.md), simply reassigning its [buffer cache key](buffer-cache-key.md) would lose those modifications. “Dirty” records a write obligation; a write of identical contents can still mark the structure dirty. Repeated buffered writes can leave only the latest contents to be transferred.

## ↑ Ancestors (6)

1. [Buffered device block](buffered-device-block.md)
2. [Buffer cache](buffer-cache.md)
3. [File system](file-system.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Buffer cache](buffer-cache.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Buffer cache validity](buffer-cache-validity.md)
- [Buffer cache writeback](buffer-cache-writeback.md)
