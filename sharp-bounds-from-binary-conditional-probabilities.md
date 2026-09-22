# Sharp bounds from binary conditional probabilities

↑ **Parent:** [Law of total probability](law-of-total-probability.md)

Write $q=P(A)$, $r=P(B\mid A)$ and $s=P(B\mid A^c)$. The [law of total probability](law-of-total-probability.md) gives the displayed [convex combination](convex-combination.md). With $q,r$ fixed and $s$ free in $[0,1]$,

$$
qr\leq P(B)\leq qr+1-q.
$$

With $r,s$ fixed and $q$ free in $[0,1]$,

$$
\min(r,s)\leq P(B)\leq\max(r,s).
$$

The joint cell masses $qr,q(1-r),(1-q)s,(1-q)(1-s)$ are nonnegative and sum to one, proving sharpness in the joint-model interpretation. For ordinary [conditional probabilities](conditional-probability.md), a conditioning event must have positive mass. If both $r$ and $s$ are specified by ratios, then $0<q<1$: for $r\ne s$ the last bounds are strict and their endpoints are the infimum and supremum. If $r=s$, the marginal equals that common value for every $q$. Endpoint mixtures remain meaningful if the unused zero-mass conditional is treated as a prescribed conditional model rather than a defined ratio.

## ↑ Ancestors (8)

1. [Law of total probability](law-of-total-probability.md)
2. [Probability measure](probability-measure.md)
3. [Probability space](probability-space-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/17/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/17/c/ii/solution.md)
