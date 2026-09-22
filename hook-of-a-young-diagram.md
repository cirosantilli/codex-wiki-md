# Hook of a Young diagram

↑ **Parent:** [Young diagram](young-diagram.md)

In the English convention of [Young diagram](young-diagram.md), the hook at a cell $(i,j)$ consists of that cell itself, all cells to its right in the same row, and all cells below it in the same column:

$$
H_{i,j}(\lambda)=\{(i,j)\}
\cup\{(i,k):j<k\leq\lambda_i\}
\cup\{(k,j):i<k\leq\lambda'_j\}.
$$

Here $\lambda'$ is the [conjugate partition](conjugate-partition.md). The cells to the right form the [arm of a Young-diagram cell](arm-of-a-young-diagram-cell.md), and those below form the [leg of a Young-diagram cell](leg-of-a-young-diagram-cell.md). Both extend all the way to the edge of the [Young diagram](young-diagram.md), rather than containing just the immediate neighbors. The three pieces are disjoint, so their total [cardinality](cardinality.md) is one plus the two lengths.

For $(3,2)$, the highlighted [Young-diagram hook](hook-of-a-young-diagram.md) is $H_{1,2}=\{(1,2),(1,3),(2,2)\}$, of [hook length](hook-length.md) three. The hook at $(1,1)$ is $\{(1,1),(1,2),(1,3),(2,1)\}$, of [hook length](hook-length.md) four: the southeast cell $(2,2)$ is excluded because it is in neither the anchor's row nor its column. These local shapes are useful because their [hook lengths](hook-length.md) give the denominator of the [hook-length formula](hook-length-formula.md). The hook terminology and its use to calculate [representation](group-representation.md) degrees appear explicitly in §1 of [Frame, Robinson and Thrall's original paper](https://doi.org/10.4153/CJM-1954-030-1).

**Table of contents**

- [Arm of a Young-diagram cell](arm-of-a-young-diagram-cell.md)
- [Leg of a Young-diagram cell](leg-of-a-young-diagram-cell.md)
- [Hook length](hook-length.md)
  - [Hook graph of a partition](hook-graph-of-a-partition.md)
    - [Hook product of a partition](hook-product-of-a-partition.md)
- [Hook-interval decomposition at a Young-diagram cell](hook-interval-decomposition-at-a-young-diagram-cell.md)
- [Divisor closure of hook lengths](divisor-closure-of-hook-lengths.md)
- [Rim hook](rim-hook.md)
  - [Border-strip tableau](border-strip-tableau.md)

## ↑ Ancestors (8)

1. [Young diagram](young-diagram.md)
2. [Partition of an integer](partition-of-an-integer.md)
3. [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group-split.md)
4. [Representation theory](representation-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Arm of a Young-diagram cell](arm-of-a-young-diagram-cell.md)
- [Greene–Nijenhuis–Wilf hook walk](greene-nijenhuis-wilf-hook-walk.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-3/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-4/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-5/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-160/3/a/i/solution.md)
