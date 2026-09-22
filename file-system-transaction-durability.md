# File-system transaction durability

↑ **Parent:** [File-system transaction](file-system-transaction.md)

An acknowledged [file-system transaction](file-system-transaction.md) remains recoverable after a crash under the stated storage assumptions. In the full-data timeline, durable [journal payload](journal-payload.md) and a durable [journal commit record](journal-commit-record.md) suffice even before the [journal checkpoint](journal-checkpoint.md). A crash before durable commit can lose the append while still preserving [file-system crash consistency](file-system-crash-consistency.md). A successful ordinary write may only have reached a [buffer cache](buffer-cache.md); an application requiring persistence must use its documented interface and check errors. On [Linux kernel](linux-kernel.md)-based systems, [fsync](fsync.md) on a [file descriptor](file-descriptor.md) persists the associated [file](computer-file.md) contents and [file metadata](file-metadata.md), but persisting a newly created name also requires [fsync](fsync.md) on the containing [file-system directory](file-system-directory.md).[fsync(2) — Linux manual page by Linux man-pages project](fsync-2-linux-manual-page-by-linux-man-pages-project.md)

**Table of contents**

- [fsync](fsync.md)

## ↑ Ancestors (6)

1. [File-system transaction](file-system-transaction.md)
2. [File-system journaling](file-system-journaling.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Buffer cache](buffer-cache.md)
- [Buffer cache access trace](buffer-cache-access-trace.md)
- [File-system journaling](file-system-journaling.md)
- [File-system transaction](file-system-transaction.md)
- [fsync](fsync.md)
