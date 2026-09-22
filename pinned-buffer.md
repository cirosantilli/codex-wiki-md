# Pinned buffer

↑ **Parent:** [Buffered device block](buffered-device-block.md)

A [buffered device block](buffered-device-block.md) whose identity is retained for unfinished work. [Reference counting](reference-counting.md) can represent both client references and additional pins. Dropping a client reference does not release an outstanding journal pin; dropping a pin does not remove somebody else's reference. In the [buffer cache state model](buffer-cache-state-model.md), $r$ counts all such retained references, so $r>0$ prevents [buffer cache eviction](buffer-cache-eviction.md). This count keeps the structure alive; a [mutex](mutex.md) separately controls who can inspect or change its contents. Waiting callers also need lifetime protection.

## ↑ Ancestors (6)

1. [Buffered device block](buffered-device-block.md)
2. [Buffer cache](buffer-cache.md)
3. [File system](file-system.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Buffer cache](buffer-cache.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
