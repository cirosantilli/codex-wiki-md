<h1 id="22i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On $C_c^0(\mathbb R^n)$ equipped with the $L^\infty$ norm, point evaluation is linear and satisfies

$$
|\Lambda f|=|f(0)|\leq\|f\|_\infty,
$$

with equality for a compactly supported function equal to one near zero. Thus $\|\Lambda\|=1$. The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) extends it, without increasing its norm, to a continuous functional $\widetilde\Lambda$ on $L^\infty(\mathbb R^n)$.

This extension cannot be represented by an $L^1$ function. If $h\in L^1$ satisfied $\widetilde\Lambda(f)=\int fh$, choose continuous functions $0\leq f_k\leq1$ with $f_k(0)=1$ and support in the ball of radius $1/k$. Then

$$
1=\widetilde\Lambda(f_k)=\int f_kh\longrightarrow0
$$

by the [absolute continuity of the Lebesgue integral](../../../../../../absolute-continuity-of-the-lebesgue-integral.md), a contradiction. Therefore $(L^\infty)'$ strictly contains the functionals represented by $L^1$; this is a [singular functional on L infinity](../../../../../../singular-functional-on-l-infinity.md).

Finally, $L^p(\mathbb R^n)$ is a [reflexive Banach space](../../../../../../reflexive-banach-space.md) exactly when

$$
1<p<\infty.
$$

The endpoint spaces $L^1$ and $L^\infty$ are not reflexive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22I](../../22i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
