# File-system journaling mode

↑ **Parent:** [File-system journaling](file-system-journaling.md)

Which contents pass through the journal and which persistence dependencies accompany them. The [ext4](ext4.md) documentation distinguishes these modes: [file metadata](file-metadata.md) and contents both pass through the journal in `data=journal`; only [file metadata](file-metadata.md) is journaled in `data=ordered`, with associated contents forced to final locations before metadata commit; only [file metadata](file-metadata.md) is journaled in `data=writeback`, without that data-before-commit dependency.[ext4 General Information by The kernel development community](ext4-general-information-by-the-kernel-development-community.md)

For our append, full data journaling uses the three-record model. Ordered metadata journaling protects $I,B$ in the journal and first persists $D$ directly in free block 9. Before commit, changing an unreferenced free block does not change the visible old [file](computer-file.md); after commit, [journal replay](journal-replay.md) supplies the new [file metadata](file-metadata.md) and the new contents are already durable. Without that dependency, recovery can produce correct allocation and size but stale contents in block 9. Ordered metadata journaling does not give general all-or-nothing contents for overwrites of already allocated [file data blocks](file-data-block.md), nor does it combine arbitrary application writes into a [file-system transaction](file-system-transaction.md). The choice of protected records determines the scope of the guarantee.

## ↑ Ancestors (5)

1. [File-system journaling](file-system-journaling.md)
2. [File system](file-system-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [ext4](ext4.md)
- [File-system journaling](file-system-journaling.md)
