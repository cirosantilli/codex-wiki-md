<h1 id="9d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\sin0=0$, the [derivative](../../../../../../derivative.md) identity $\sin'=\cos$, [continuity](../../../../../../continuous-function.md) of cosine at zero, and $\cos0=1$. For $u\ne0$, the [mean value theorem](../../../../../../mean-value-theorem.md) gives $\sin u/u=\cos c_u$ for a point between zero and $u$. Hence $\sin u/u\to1$ as $u\to0$. For $x\ne0$, apply this with $u=x/3^k$ to obtain **the limit** $\boxed{3^k\sin(x/3^k)\to x}$. For $x=0$ every term is zero.

The additional bound $|\cos t|\leq1$ and the same [mean value theorem](../../../../../../mean-value-theorem.md) give $|\sin u|\leq|u|$. Therefore

$$
2^n\left|\sin\left(\frac x{3^n}\right)\right|\leq|x|\left(\frac23\right)^n.
$$

The right side is summable. By the [comparison test for series](../../../../../../comparison-test-for-series.md) **the stated series has [absolute convergence](../../../../../../absolute-convergence.md) for every real $x$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
