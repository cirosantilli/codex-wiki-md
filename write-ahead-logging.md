# Write-ahead logging

↑ **Parent:** [File-system journaling](file-system-journaling.md)

Making a recoverable journal entry durable before installing its protected updates at their final locations. In this article the journal contains new record images, so recovery redoes committed changes rather than undoing uncommitted changes. The diagrams assume one isolated [file-system transaction](file-system-transaction.md), fresh journal slots with unambiguous record identities, no other writer, and [atomic storage writes](atomic-storage-write.md) for each record and marker. A crash loses volatile state; previously durable contents remain intact. [Storage flushes](storage-flush.md) are honored, and recovery finishes before the [file system](file-system-split.md) is exposed. These are model assumptions, not a claim that every physical [file data block](file-data-block.md) write is indivisible on arbitrary hardware.

**Table of contents**

- [Journal payload](journal-payload.md)
- [Journal commit record](journal-commit-record.md)
- [Journal checkpoint](journal-checkpoint.md)
- [Journal replay](journal-replay.md)

## ↑ Ancestors (5)

1. [File-system journaling](file-system-journaling.md)
2. [File system](file-system-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Buffer cache state model](buffer-cache-state-model.md)
- [File-system journaling](file-system-journaling.md)
