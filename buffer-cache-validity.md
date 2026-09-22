# Buffer cache validity

↑ **Parent:** [Buffered device block](buffered-device-block.md)

Whether a [buffered device block](buffered-device-block.md)'s contents are ready for the requested use. Reserving a [buffer cache key](buffer-cache-key.md) does not make its previous occupant's contents valid. A read fills the reserved structure before exposing its contents. A second caller finding an unfinished fill must wait; finding the identity is not yet a data [cache hit](cache-hit.md) under the convention used here. A failed fill must not expose the stale contents as valid.

A buffered partial write first needs the untouched [bytes](byte.md): read the old contents on a [cache miss](cache-miss.md), change the requested range, and retain the result as a [dirty buffer](dirty-buffer.md). A complete overwrite can initialize every [byte](byte.md) without reading the old contents if the interface permits that path. The [buffer cache access trace](buffer-cache-access-trace.md) deliberately uses partial writes, so every [cache miss](cache-miss.md) reads the old block.

## ↑ Ancestors (6)

1. [Buffered device block](buffered-device-block.md)
2. [Buffer cache](buffer-cache.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Buffer cache state model](buffer-cache-state-model.md)
- [Buffered device block](buffered-device-block.md)
