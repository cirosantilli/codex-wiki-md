<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

[NTFS](../../../../../../ntfs.md) offers several capabilities absent from [FAT32](../../../../../../fat32.md). Four relevant advantages are **per-file security, recoverable metadata updates, larger files and transparent compression**. In detail, [access control lists](../../../../../../access-control-list.md) and ownership allow different users to have different rights on individual objects; [file-system journaling](../../../../../../file-system-journaling.md) helps recover a consistent metadata structure after a crash; file sizes can exceed FAT32's limit of $2^{32}-1$ bytes per file; and built-in compression can reduce the storage needed without changing application file access.

Encryption, quotas and sparse-file support are additional examples, but are not needed for the four requested points. Metadata journaling is not the same as guaranteeing that every recent data write survives a failure, and superiority in these capabilities does not mean universal superiority in compatibility or simplicity. The supported features are compared in [the filesystem functionality documentation](https://learn.microsoft.com/en-us/windows/win32/fileio/filesystem-functionality-comparison).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [8](../../8.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
