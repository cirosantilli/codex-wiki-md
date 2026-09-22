<h1 id="18/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $f\in L^2[-L,L]$, so the squared-error [integral](../../../../../integral-split.md) is finite. Write

$$
r_N(x)=f(x)-\frac{a_0}{2}-\sum_{n=1}^Na_n\cos\frac{n\pi x}{L}.
$$

At a minimum, differentiating with respect to each coefficient gives

$$
0=\frac{\partial F}{\partial a_0}=-\int_{-L}^Lr_N(x)dx,
\qquad
0=\frac{\partial F}{\partial a_m}=-2\int_{-L}^Lr_N(x)\cos\frac{m\pi x}{L}dx.
$$

By [Fourier orthogonality](../../../../../fourier-orthogonality.md), the constant has squared norm $2L$, each nonconstant cosine has squared norm $L$, and all distinct modes are orthogonal. Thus

$$
\boxed{a_0=\frac1L\int_{-L}^Lf(x)dx,\qquad
 a_n=\frac1L\int_{-L}^Lf(x)\cos\frac{n\pi x}{L}dx\quad(1\leq n\leq N).}
$$

These are exactly the [Fourier coefficients](../../../../../fourier-coefficient.md) of the [Fourier cosine series](../../../../../fourier-cosine-series.md) of the [even function](../../../../../even-function.md). To check that the stationary choice is a unique global minimum, perturb the coefficients by $\delta a_n$. The residual is orthogonal to every fitted mode, so the cross terms vanish and

$$
F(\boldsymbol a+\delta\boldsymbol a)-F(\boldsymbol a)
=\frac L2(\delta a_0)^2+L\sum_{n=1}^N(\delta a_n)^2\geq0,
$$

with equality only when every perturbation is zero. The truncated series is the [orthogonal projection onto a finite-dimensional subspace](../../../../../orthogonal-projection-onto-a-finite-dimensional-subspace.md) spanned by the constant and the first $N$ cosine modes.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
