<h1 id="23i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the [Fourier transform](../../../../../../fourier-transform.md) of the equation in the sense of [distributions](../../../../../../distribution-mathematical-analysis.md) gives

$$
(|\xi|^4-|\xi|^2+1)\widehat u(\xi)=\widehat f(\xi).
$$

The [Fourier multiplier](../../../../../../fourier-multiplier.md)

$$
m(\xi)=|\xi|^4-|\xi|^2+1=\left(|\xi|^2-\frac12\right)^2+\frac34
$$

is everywhere positive. Define $\widehat u=\widehat f/m$. Since

$$
\sup_{\xi\in\mathbb R^n}\frac{(1+|\xi|^2)^2}{m(\xi)}<\infty,
$$

we have

$$
\lVert u\rVert_{H^{s+4}}^2
=\int(1+|\xi|^2)^{s+4}\frac{|\widehat f(\xi)|^2}{m(\xi)^2}\,d\xi
\leq C^2\lVert f\rVert_{H^s}^2.
$$

Thus $u\in H^{s+4}$ exists and obeys the required estimate. If two solutions existed, their difference would have $m\widehat u=0$; positivity of $m$ proves uniqueness.

A [classical solution](../../../../../../classical-solution.md) needs continuous derivatives through order four. Applying the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) with $k=4$ to $u\in H^{s+4}$ shows that this is guaranteed when

$$
s+4>4+\frac n2,
$$

or equivalently

$$
\boxed{s>\frac n2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23I](../../23i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
