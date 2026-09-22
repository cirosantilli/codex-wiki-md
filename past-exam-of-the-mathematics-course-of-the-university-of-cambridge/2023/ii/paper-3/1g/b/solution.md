<h1 id="1g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [Chebyshev theta function](../../../../../../chebyshev-theta-function.md) as

$$
\vartheta(x)=\sum_{\substack{p\leq x\\p\text{ prime}}}\log p.
$$

Taking [natural logarithms](../../../../../../natural-logarithm.md) in part a gives

$$
2n\log2-\log(2n+1)
\leq\sqrt{2n}\log(2n)+\vartheta(2n),
$$

and hence

$$
\vartheta(2n)\geq
2n\log2-\sqrt{2n}\log(2n)-\log(2n+1).
$$

Because $\sqrt n\log n/n\to0$, the right-hand side is at least $n/2$ for every sufficiently large [integer](../../../../../../integer.md) $n$.

Now let $x$ be sufficiently large and set $n=\lfloor x/2\rfloor$ using the [floor function](../../../../../../floor-function.md). Then $2n\leq x$ and $n\geq x/3$, so the monotonicity of $\vartheta$ gives

$$
\boxed{
\sum_{\substack{p\leq x\\p\text{ prime}}}\log p
=\vartheta(x)\geq\vartheta(2n)
\geq\frac n2\geq\frac{x}{6}\geq\frac{x}{12}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1G](../../1g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
