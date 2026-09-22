<h1 id="26k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the interval as $I=(c,d]$, where $0<c<d<1$, to avoid confusing its left endpoint with the rotation parameter $\alpha$. For every sufficiently large integer $k$, define an inner and outer interval on the circle by

$$
I_k^-=(c+k^{-1},d-k^{-1}],
\qquad
I_k^+=(c-k^{-1},d+k^{-1}].
$$

Apply part (b) simultaneously to this countable collection of intervals. The intersection $G$ of the corresponding full-measure sets still has full [Lebesgue measure](../../../../../../lebesgue-measure.md), and is therefore [dense](../../../../../../dense-set.md) in the circle.

Fix an arbitrary $x$. For each sufficiently large $k$, choose $y_k\in G$ with circle distance less than $1/k$ from $x$. An [irrational circle rotation](../../../../../../irrational-rotation.md) preserves this distance, so for every $j\geq0$,

$$
\mathbf1_{I_k^-}(T^jy_k)
\leq\mathbf1_I(T^jx)
\leq\mathbf1_{I_k^+}(T^jy_k).
$$

Averaging and using part (b) for $y_k$ gives

$$
d-c-\frac2k
\leq
\liminf_{n\to\infty}\frac{S_n(\mathbf1_I)(x)}n
\leq
\limsup_{n\to\infty}\frac{S_n(\mathbf1_I)(x)}n
\leq
d-c+\frac2k.
$$

Letting $k\to\infty$ proves the [everywhere interval frequency under an irrational rotation](../../../../../../everywhere-interval-frequency-under-an-irrational-rotation.md):

$$
\boxed{
\frac{S_n(\mathbf1_{(c,d]})(x)}n\longrightarrow d-c
\quad\text{for every }x\in(0,1].}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
