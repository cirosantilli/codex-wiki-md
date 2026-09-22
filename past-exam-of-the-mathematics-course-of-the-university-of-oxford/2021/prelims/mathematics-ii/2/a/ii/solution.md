<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\varepsilon>0$. By the definition of [Cauchy sequence](../../../../../../../cauchy-sequence.md), choose an [integer](../../../../../../../integer-split.md) $K\geq1$ such that $|x_j-x_k|<\varepsilon/2$ whenever $j,k\geq K$. Apply the given [inequality](../../../../../../../inequality-mathematics.md) with $N=K+1$. It supplies $n>K+1$ for which

$$
0<x_n\leq\frac12\min_{k<K+1}x_k\leq\frac{x_K}{2}.
$$

Both $n$ and $K$ are in the [Cauchy sequence](../../../../../../../cauchy-sequence.md) estimate, so

$$
\frac{x_K}{2}\leq x_K-x_n<\frac\varepsilon2,
\qquad\text{hence}\qquad x_n<\frac\varepsilon2.
$$

For every $m\geq K$ the [triangle inequality](../../../../../../../triangle-inequality.md) gives

$$
0<x_m\leq|x_m-x_n|+x_n<\varepsilon.
$$

This is the definition of [convergence](../../../../../../../convergence.md) to zero: $\boxed{x_m\to0}$. The proof uses only the [Cauchy sequence](../../../../../../../cauchy-sequence.md) estimate, positivity, and the stipulated [inequality](../../../../../../../inequality-mathematics.md); it does not assume the general [completeness of the real numbers](../../../../../../../completeness-of-the-real-numbers.md) theorem for [Cauchy sequences](../../../../../../../cauchy-sequence.md). Taking $N=K+1\geq2$ also avoids the empty initial [set](../../../../../../../set-split.md) in a literal reading of the condition for very small $N$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
