# First row of RSK as a minimum-tail table

↑ **Parent:** [Minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md)

For a [permutation](permutation.md) input, the first row of its [RSK](robinson-schensted-knuth-correspondence.md) insertion tableau is the [minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md): its $j$th entry is the least attainable final value of a [strictly increasing subsequence](strictly-increasing-subsequence.md) of [length](length.md) $j$ in the processed prefix. Inserting $z$ replaces the first entry larger than $z$, or appends if none exists. In replacement position $r$, the previous entry in position $r-1$ supplies a subsequence that can be extended by $z$. Shorter [minimum](minimum-of-a-subset-of-a-total-order.md) tails were already smaller, and a longer subsequence ending at $z$ would require an old tail in position at least $r$ smaller than $z$, contrary to the replacement rule. This proves the [invariant](invariant-mathematics.md) inductively. Consequently the first-row [length](length.md) is the [longest increasing subsequence](longest-increasing-subsequence.md) [length](length.md). The row entries need not be a subsequence together: input $2,4,3,1$ gives first row $1,3$, although one occurs after three. They are minima for different lengths, obtained from potentially different subsequences.

## ↑ Ancestors (7)

1. [Minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md)
2. [Longest increasing subsequence](longest-increasing-subsequence.md)
3. [Increasing subsequence](increasing-subsequence.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford/2011/3/d/solution.md)
