<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An [inode](../../../../../../inode.md) is a filesystem object record, identified by its inode number. It contains file type and mode bits, owner/group identifiers, link count, file size, timestamps and the information locating data blocks. It normally does not contain the filename: directory entries map names to inode numbers, allowing several names to refer to one inode. In the traditional Unix layout, there are direct block pointers and single-, double- and triple-indirect pointers. A single-indirect block points to data blocks; a double-indirect block points to single-indirect blocks; the triple-indirect level adds one further pointer layer.

Let $D$ be the number of direct pointers. Before triple indirection is needed, the file can use $D$ directly addressed data blocks, 512 singly addressed data blocks and $512^2$ doubly addressed data blocks. Indirection blocks consume disk space but are not part of the file's logical byte contents. Hence

$$
\boxed{\text{maximum file size without triple indirection}=4096\big(D+512+512^2\big)\text{ bytes}.}
$$

The PDF does not specify $D$. With the common twelve-direct-pointer convention, this is $4096(12+512+512^2)=1{,}075{,}888{,}128$ bytes; with ten direct pointers, substitute $D=10$. The formula, rather than an unstated choice of direct-pointer count, determines the answer for the given inode layout. Actual filesystems can use other pointer organizations such as extents.

## ↑ Ancestors (11)

1. [D](../d.md)
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
