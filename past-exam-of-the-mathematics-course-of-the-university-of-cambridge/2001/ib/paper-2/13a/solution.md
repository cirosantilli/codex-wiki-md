<h1 id="13a/solution">Solution</h1>

↑ **Parent:** [13A](../13a.md)

The [Liouville theorem](../../../../../liouville-theorem.md) states that every bounded [entire function](../../../../../entire-function.md) is constant. Let $|f(z)|\le M$ and choose distinct $a,b$. For $R>\max(|a|,|b|)$, partial fractions and the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) give

$$
I_R=\int_{|z|=R}\frac{f(z)}{(z-a)(z-b)}\,dz
=\frac{2\pi i}{a-b}[f(a)-f(b)],
$$

with the circle traversed anticlockwise. On that circle,

$$
|I_R|\le\frac{2\pi RM}{(R-|a|)(R-|b|)}\longrightarrow0.
$$

The displayed difference is independent of $R$, so $f(a)=f(b)$. Since $a,b$ were arbitrary, **$f$ is constant**. This proves the theorem with the requested two-pole contour rather than assuming it.

## ↑ Ancestors (10)

1. [13A](../13a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
