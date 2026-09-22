# Clean buffer

↑ **Parent:** [Buffered device block](buffered-device-block.md)

A valid [buffered device block](buffered-device-block.md) with no outstanding write obligation to the backing location tracked by this cache. It can serve a [cache hit](cache-hit.md). It becomes eligible for [buffer cache eviction](buffer-cache-eviction.md) only when its retention and any pending [input-output](input-output.md) permit reuse. “Clean” does not assert that a device's volatile [memory cache](cache-computing.md) has been flushed to persistent storage.

## ↑ Ancestors (6)

1. [Buffered device block](buffered-device-block.md)
2. [Buffer cache](buffer-cache.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Buffer cache](buffer-cache.md)
- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Buffer cache writeback](buffer-cache-writeback.md)
