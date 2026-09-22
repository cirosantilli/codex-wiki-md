# Atomic storage write

↑ **Parent:** [File system](file-system-split.md)

A write whose durable result after a crash is either the complete old record or the complete new record. Its unit and failure conditions must be stated. The diagrams assume this property for each payload record, final-location record, commit marker and retirement marker; they do not derive it from the size of a [file data block](file-data-block.md).

## ↑ Ancestors (4)

1. [File system](file-system-split.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Journal replay](journal-replay.md)
- [Memory-mapped file synchronization](memory-mapped-file-synchronization.md)
- [Storage flush](storage-flush.md)
- [Write-ahead logging](write-ahead-logging.md)
