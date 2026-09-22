# Copy-on-write page accounting

↑ **Parent:** [Copy-on-write](copy-on-write.md)

Assume exactly two [operating-system processes](process-computing.md), $N$ initially resident private [memory pages](memory-page.md) of $P$ [bytes](byte.md) each, initially distinct [page frames](page-frame.md) shared by A and B. Neither unmaps, exits, forks again, or encounters [page replacement](page-replacement.md); no other owner exists, allocation succeeds, and a first write copies one whole shared [memory page](memory-page.md). Once a [page frame](page-frame.md) is exclusively owned it is reused on writes, without another copy; writable mappings remain writable. Count data storage only, excluding [page tables](page-table.md) and other bookkeeping. With B as the only writer, writing $k$ distinct [memory pages](memory-page.md) gives

$$
\text{new allocations}=\text{whole-page copies}=k,\qquad \text{resident data bytes}=(N+k)P.
$$

This depends on distinct written [memory pages](memory-page.md), not the number of store instructions or reads. For the diagrams, take $N=3$ and an illustrative $P=4096$ [bytes](byte.md):

| Access pattern | New [page frames](page-frame.md) | Whole-page copies | Resident data [bytes](byte.md) |
| --- | --- | --- | --- |
| Both only read | 0 | 0 | 12288 |
| B writes [memory page](memory-page.md) `0x12` once | 1 | 1 | 16384 |
| B writes [memory page](memory-page.md) `0x12` one hundred times | 1 | 1 | 16384 |
| B writes [memory pages](memory-page.md) `0x12` and `0x14` | 2 | 2 | 20480 |
| B writes all three [memory pages](memory-page.md) | 3 | 3 | 24576 |
| B then A each write [memory page](memory-page.md) `0x12` | 1 | 1 | 16384 |

For both writers, let $S_A,S_B$ be the [sets](set-split.md) of initial [memory page](memory-page.md) numbers written by A and B. Under these assumptions, new allocations and copies both equal $|S_A\cup S_B|$, the [cardinality](cardinality.md) of their [set union](set-union.md), while resident data storage is $(N+|S_A\cup S_B|)P$. Each initially shared [page frame](page-frame.md) needs at most one split: after the first writer copies it, the other owns the original exclusively. Both writing the same [memory page](memory-page.md) therefore produces two versions with one copy, even if the final values happen to match. The last row can incur two protection [page faults](page-fault.md), one for each writer, while making only one copy. A handler that always allocates on a protected write can make a second copy and free the now-unreferenced original: allocation counts and final resident storage are different observables.

These are model counts, not measured Linux costs or a guaranteed bound on total [computer memory](computer-memory.md). More descendants, other owners, [demand paging](demand-paging.md), [page replacement](page-replacement.md), different [memory page](memory-page.md) sizes, and different exclusive-ownership rules change the accounting. The useful claim is conditional: deferred data copying can cost in proportion to the distinct shared [memory pages](memory-page.md) that are written, while creating separate [page tables](page-table.md) has its own cost.

// Target: computer-science.bigb

## ↑ Ancestors (5)

1. [Copy-on-write](copy-on-write.md)
2. [Virtual memory](virtual-memory-split.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Copy-on-write fault handling](copy-on-write-fault-handling.md)
