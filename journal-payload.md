# Journal payload

↑ **Parent:** [Write-ahead logging](write-ahead-logging.md)

The protected new contents and destination information for a [file-system transaction](file-system-transaction.md). In the diagrams, the three complete [journal payload](journal-payload.md) records correspond to $I,B,D$. Records can reach storage in any order within this phase. The [journal commit record](journal-commit-record.md) cannot become durable until all three are durable.

## ↑ Ancestors (6)

1. [Write-ahead logging](write-ahead-logging.md)
2. [File-system journaling](file-system-journaling.md)
3. [File system](file-system-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [File-system journaling](file-system-journaling.md)
- [File-system transaction durability](file-system-transaction-durability.md)
- [Journal checkpoint](journal-checkpoint.md)
- [Journal commit record](journal-commit-record.md)
- [Journal payload](journal-payload.md)
- [Journal replay](journal-replay.md)
