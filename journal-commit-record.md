# Journal commit record

↑ **Parent:** [Write-ahead logging](write-ahead-logging.md)

A marker identifying a complete committed [file-system transaction](file-system-transaction.md). A marker alone is insufficient if its [journal payload](journal-payload.md) is missing or belongs to another group. The simple model prevents this through ordering and fresh record identities. Real journal formats also validate record identities and integrity: the [ext4](ext4.md) documentation says replay discards a group lacking its commit or having mismatched integrity checks.[3.6. Journal (jbd2) by The kernel development community](3-6-journal-jbd2-by-the-kernel-development-community.md)

## ↑ Ancestors (6)

1. [Write-ahead logging](write-ahead-logging.md)
2. [File-system journaling](file-system-journaling.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [File-system journaling](file-system-journaling.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [Journal payload](journal-payload.md)
