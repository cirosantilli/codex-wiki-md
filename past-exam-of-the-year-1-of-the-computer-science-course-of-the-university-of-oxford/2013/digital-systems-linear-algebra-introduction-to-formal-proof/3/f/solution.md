<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let a [disk block number](../../../../../disk-block-number.md) and a file number each occupy $h$ bytes. System B spends about $3h$ bytes per physical block on successor/count, predecessor and owner, leaving $B-3h$ payload bytes. It also needs its per-file header. In the traditional [inode](../../../../../inode.md) scheme, [file data blocks](../../../../../file-data-block.md) are entirely payload; indexing occupies the fixed [inode](../../../../../inode.md) and separate indirect blocks.

For $N$ data blocks in a large densely occupied indirect tree, about $N/q$ lowest-level index blocks, $N/q^2$ next-level blocks and so on are needed. With $q=B/h$, the asymptotic indexing space is approximately

$$
B\left(\frac Nq+\frac N{q^2}+\cdots\right)\approx\frac{NB}{q-1},
$$

or about $Nh$ bytes when $q$ is large. Thus

$$
\boxed{\text{large-file UNIX indexing is roughly one address per data block, versus three fields in System B}.}
$$

This is a comparison of typical densely used structures. For a small file, the fixed [inode](../../../../../inode.md) dominates; near an indirect-level boundary, partly empty index blocks add overhead. Both schemes can waste part of the last block through [internal fragmentation](../../../../../internal-fragmentation.md).

The main performance advantage is indexed access to an arbitrary [file offset](../../../../../file-offset.md): the [inode](../../../../../inode.md) finds the required data block with at most three indirect levels, whereas System B may need to follow a long chain from one end. Index blocks can be cached and scanned in batches, leaving complete data blocks for transfers. The [inode](../../../../../inode.md) scheme also naturally supports [sparse files](../../../../../sparse-file.md), where absent data-block pointers represent zero-filled holes without allocating every intervening block.

There are additional costs. A cold lookup can require separate index-block reads, allocation near a boundary can require allocating and updating several index blocks, and small files can pay more fixed metadata cost. System B already has a tail pointer and can append with local chain updates, while its owner and predecessor fields can help recovery from surviving blocks. Losing a UNIX indirect block can disconnect many data blocks, and those blocks do not automatically carry System B's owner information. Thus the space and [file offset](../../../../../file-offset.md) access advantages do not imply uniformly cheaper updates or uniformly better recovery.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
