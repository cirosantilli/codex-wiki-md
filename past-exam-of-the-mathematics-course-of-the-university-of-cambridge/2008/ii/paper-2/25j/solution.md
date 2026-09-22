<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

A [simple function](../../../../../simple-function.md) is a [measurable function](../../../../../measurable-function.md) taking finitely many values, expressible as $s=\sum_{j=1}^ma_j1_{A_j}$ for disjoint measurable sets. For nonnegative coefficients define $\int s\,d\mu=\sum_ja_j\mu(A_j)$. The [Lebesgue integral](../../../../../lebesgue-integral.md) of a nonnegative measurable $f$ is

$$
\boxed{\int f\,d\mu=\sup\{\int s\,d\mu:0\le s\le f,\ s\text{ simple}\}.}
$$

Suppose $0\le g_n\uparrow f$ with each $g_n$ simple. Their integrals increase and are bounded above by $\int f$. For the reverse bound, fix any simple $0\le s\le f$ and $0<c<1$. The sets $E_n=\{g_n\ge cs\}$ increase to a set containing $\{s>0\}$. Hence $\int g_n\ge c\int s1_{E_n}$, whose right side tends to $c\int s$ by continuity from below of the measure on the finitely many level sets of $s$. Let $c\uparrow1$ and then take the supremum over $s$. This proves $\int g_n\uparrow\int f$, including infinite limiting integrals.

The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) states the same conclusion for any nonnegative measurable sequence $f_n\uparrow f$, without simplicity. The preceding lower-bound argument works unchanged: $E_n=\{f_n\ge cs\}$ and monotonicity of the integral give $\int f_n\ge c\int s1_{E_n}$. Taking limits and the same two suprema proves

$$
\boxed{\lim_n\int f_n\,d\mu=\int\lim_n f_n\,d\mu.}
$$

The upper bound follows from $f_n\le f$. Finiteness of the measure makes all bounded simple integrals finite in this proof; the theorem in fact extends to arbitrary measure spaces.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
