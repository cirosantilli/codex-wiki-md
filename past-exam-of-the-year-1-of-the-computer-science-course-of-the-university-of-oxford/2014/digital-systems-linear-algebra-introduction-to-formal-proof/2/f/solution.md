<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

With a resident [inode](../../../../../inode.md), the deepest allowed path uses two address blocks and one [file data block](../../../../../file-data-block.md), so every byte through the end of the doubly indirect region meets the three-read bound. There are ten directly addressed [file data blocks](../../../../../file-data-block.md), 512 singly addressed ones and $512^2$ doubly addressed ones. Therefore the largest contiguous [file](../../../../../computer-file.md) satisfying this bound is

$$
\boxed{2048(10+512+512^2)=537\,939\,968\text{ bytes}.}
$$

The next byte requires the triply indirect region, with three address-block reads and a fourth read for the [file data block](../../../../../file-data-block.md).

The resident-[inode](../../../../../inode.md) convention is essential. If the question's three reads must also include fetching a previously uncached [inode](../../../../../inode.md), only two further reads remain; the maximum is then

$$
\boxed{2048(10+512)=1\,069\,056\text{ bytes, if the inode read is included}.}
$$

Neither figure includes arbitrary pathname-resolution reads. These are worst-case counts in the traditional fully allocated [multilevel inode indexing](../../../../../multilevel-inode-indexing.md) model; existing [buffer cache](../../../../../buffer-cache.md) entries can reduce them.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
