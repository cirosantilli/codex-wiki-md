# Buffer cache eviction

↑ **Parent:** [Buffer cache](buffer-cache.md)

Removing a [buffer cache key](buffer-cache-key.md)'s resident contents so the storage in [computer memory](computer-memory.md) can serve another key. An unreferenced [clean buffer](clean-buffer.md) can be reused directly in the [buffer cache state model](buffer-cache-state-model.md); an unreferenced [dirty buffer](dirty-buffer.md) requires successful [buffer cache writeback](buffer-cache-writeback.md) first. A [pinned buffer](pinned-buffer.md) cannot be chosen regardless of cleanliness. [LRU replacement](lru-replacement.md) ranks eligible candidates; it does not override lifetime protection. If every candidate is retained, a [cache miss](cache-miss.md) cannot obtain space until something releases a reference or capacity changes. This is a resource shortage, not permission to discard live contents.

## ↑ Ancestors (5)

1. [Buffer cache](buffer-cache.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Buffer cache writeback](buffer-cache-writeback.md)
- [Clean buffer](clean-buffer.md)
- [Pinned buffer](pinned-buffer.md)
