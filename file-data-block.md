# File data block

↑ **Parent:** [Computer file](computer-file.md)

A storage unit holding part of a [file](computer-file.md)'s contents. The toy [inode](inode.md) references two four-[byte](byte.md) [file data blocks](file-data-block.md) for six [bytes](byte.md) of contents: allocated capacity is $2\cdot4=8$ [bytes](byte.md), while logical size is $4+2=6$ [bytes](byte.md). This counts only the two [file data blocks](file-data-block.md), excluding storage for the [inode](inode.md) and [directory entries](directory-entry.md).

## ↑ Ancestors (5)

1. [Computer file](computer-file.md)
2. [File system](file-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Atomic storage write](atomic-storage-write.md)
- [Block allocation bitmap](block-allocation-bitmap.md)
- [Buffer cache](buffer-cache.md)
- [Buffered device block](buffered-device-block.md)
- [File data block](file-data-block.md)
- [File system](file-system.md)
- [File-system journaling](file-system-journaling.md)
- [File-system journaling mode](file-system-journaling-mode.md)
- [File-system transaction](file-system-transaction.md)
- [Inode](inode.md)
- [Unlinking an open file](unlinking-an-open-file.md)
- [Write-ahead logging](write-ahead-logging.md)
