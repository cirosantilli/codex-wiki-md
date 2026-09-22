# File-system transaction

↑ **Parent:** [File-system journaling](file-system-journaling.md)

A group of updates treated as one unit for [file-system crash consistency](file-system-crash-consistency.md). The three-record append above is one explicitly chosen group. Real [file-system journaling](file-system-journaling.md) can batch several [system calls](system-call.md) or split large work across several groups; it does not automatically make an application's several writes into one [file-system transaction](file-system-transaction.md). An [atomic operation](atomic-operation.md) for competing [software threads](thread-computing.md) likewise does not by itself provide [file-system transaction durability](file-system-transaction-durability.md).

Creation shows why the group must include every related change. In a toy [file-system directory](file-system-directory.md) with space for one more name, creating `notes` with contents `EFGH` needs a [directory entry](directory-entry.md) mapping `notes` to newly allocated [inode](inode.md) 42, an [inode allocation bitmap](inode-allocation-bitmap.md) marking 42 in use, that [inode](inode.md) with size 4 and a reference to block 9, a [block allocation bitmap](block-allocation-bitmap.md) allocating 9, and [file data block](file-data-block.md) 9 with the contents. An exposed [directory entry](directory-entry.md) must reach an allocated [inode](inode.md), and its content references must reach allocated [file data blocks](file-data-block.md). Protecting just the [inode](inode.md) leaves these relationships outside the [file-system transaction](file-system-transaction.md). This simplified five-record creation excludes parent-directory growth, timestamps and allocation counters; a real [file system](file-system.md) must include its own additional dependencies.

**Table of contents**

- [File-system transaction durability](file-system-transaction-durability.md)
  - [fsync](fsync.md)

## ↑ Ancestors (5)

1. [File-system journaling](file-system-journaling.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [File-system crash consistency](file-system-crash-consistency.md)
- [File-system journaling](file-system-journaling.md)
- [File-system journaling mode](file-system-journaling-mode.md)
- [File-system transaction](file-system-transaction.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [Journal commit record](journal-commit-record.md)
- [Journal payload](journal-payload.md)
- [Journal replay](journal-replay.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
- [Write-ahead logging](write-ahead-logging.md)
