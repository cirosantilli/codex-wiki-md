# File-system crash consistency

↑ **Parent:** [File-system journaling](file-system-journaling.md)

The guarantee that recovery produces a valid [file system](file-system.md) state under a specified crash model. For the protected [file-system transaction](file-system-transaction.md) in our full-data example, the observable [file](computer-file.md) is either `ABCD` or `ABCDEFGH`; it never names a free block or exposes a half-applied protected append after recovery. This concerns the recovered state. The intermediate final-location records during a [journal checkpoint](journal-checkpoint.md) may disagree until [journal replay](journal-replay.md) finishes, and live concurrent access requires separate [synchronization](synchronization-computing.md).

## ↑ Ancestors (5)

1. [File-system journaling](file-system-journaling.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [File-system allocation bitmap](file-system-allocation-bitmap.md)
- [File-system journaling](file-system-journaling.md)
- [File-system transaction](file-system-transaction.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
- [Microkernel service failure isolation](microkernel-service-failure-isolation.md)
