<h1 id="4/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reversing the finite summations gives

$$
\frac1{n^{3/2}}\sum_{k=1}^n\sum_{j=1}^kX_j
=\frac1n\sum_{k=1}^n\frac{S_k}{\sqrt n}.
$$

This is a [Riemann sum](../../../../../../../riemann-sum.md) for the continuous functional $f\mapsto\int_0^1f(t)\,dt$ evaluated at the interpolated random walk; the interpolation error tends to zero in probability. The [continuous mapping theorem](../../../../../../../continuous-mapping-theorem.md) and part (b) yield

$$
\boxed{\frac1{n^{3/2}}\sum_{k=1}^n\sum_{j=1}^kX_j
\xrightarrow d\int_0^1B_t\,dt
\sim N(0,1/3).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
