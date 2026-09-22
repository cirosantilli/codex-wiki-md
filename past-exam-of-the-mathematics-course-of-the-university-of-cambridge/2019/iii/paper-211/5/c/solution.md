<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $T\mapsto P_t^T$ is nonincreasing, then

$$
P_t^{t+1}\leq P_t^t=1,
$$

so $1+r_t=(P_t^{t+1})^{-1}\geq1$ and $r_t\geq0$.

Conversely, if every spot rate is nonnegative, then $B_{T+1}=B_T(1+r_T)\geq B_T$. Under a [risk-neutral measure](../../../../../../risk-neutral-measure.md),

$$
P_t^{T+1}
=B_t\mathbb E^Q[B_{T+1}^{-1}\mid\mathcal F_t]
\leq B_t\mathbb E^Q[B_T^{-1}\mid\mathcal F_t]
=P_t^T.
$$

Hence

$$
\boxed{T\mapsto P_t^T\text{ is nonincreasing}
\iff r_t\geq0\text{ for every }t.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
