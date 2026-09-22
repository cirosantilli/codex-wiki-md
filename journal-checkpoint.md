# Journal checkpoint

↑ **Parent:** [Write-ahead logging](write-ahead-logging.md)

Installing committed [journal payload](journal-payload.md) at final locations and making those copies durable. Safe retirement follows this completion, not merely submission of the copies. Discarding the journal while some copies remain only in a volatile [memory cache](cache-computing.md) can leave an unrecoverable mixture after a crash. Commit establishes a recoverable decision; a [journal checkpoint](journal-checkpoint.md) permits reclamation of its journal space.

## ↑ Ancestors (6)

1. [Write-ahead logging](write-ahead-logging.md)
2. [File-system journaling](file-system-journaling.md)
3. [File system](file-system.md)
4. [Operating system](operating-system.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [File-system backup](file-system-backup.md)
- [File-system crash consistency](file-system-crash-consistency.md)
- [File-system journaling](file-system-journaling.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [Journal checkpoint](journal-checkpoint.md)
- [Journal replay](journal-replay.md)
