<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use degree-indexed [Fourier partial sums](../../../../../../fourier-partial-sum.md) and [Fejér sums](../../../../../../fejer-sum.md), as in this paper. For a $2\pi$-periodic [continuous function](../../../../../../continuous-function.md), put

$$
\widehat f_k=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-ikt}\,dt,\qquad s_n(f,x)=\sum_{k=-n}^n\widehat f_ke^{ikx},\qquad \sigma_n(f)=\frac1{n+1}\sum_{j=0}^ns_j(f).
$$

Equivalently,

$$
\sigma_n(f,x)=\sum_{|k|\le n}\left(1-\frac{|k|}{n+1}\right)\widehat f_ke^{ikx}.
$$

These are [trigonometric polynomials](../../../../../../trigonometric-polynomial.md) of degree at most $n$. Some treatments index the [Fejér sum](../../../../../../fejer-sum.md) by the number of terms rather than its degree; the degree convention here is why the formulas below contain $\sigma_{2n-1}$ and $\sigma_{n-1}$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
