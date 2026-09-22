<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $K=k+1$ and $h_j=\mathbb E_jD_j$. The [expected duration of symmetric gambler's ruin](../../../../../../expected-duration-of-symmetric-gambler-s-ruin.md) satisfies $h_0=h_K=0$ and, by conditioning on the first step,

$$
h_j=1+\frac12h_{j-1}+\frac12h_{j+1},\qquad1\leq j\leq K-1.
$$

These [expected values](../../../../../../expected-value.md) are finite: from any interior state, $K$ consecutive right steps ensure absorption, an event of probability at least $2^{-K}$. Blocks of $K$ steps therefore bound the survival probability by a decreasing geometric sequence. The candidate $h_j=j(K-j)$ has the required boundary values and satisfies $h_{j+1}-2h_j+h_{j-1}=-2$. Hence

$$
\boxed{\mathbb E D_j=j(k+1-j).}
$$

For completeness, the difference of two solutions of this [linear recurrence relation](../../../../../../linear-recurrence-relation.md) has zero second difference and is affine in $j$; its two zero boundary values force it to vanish.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
