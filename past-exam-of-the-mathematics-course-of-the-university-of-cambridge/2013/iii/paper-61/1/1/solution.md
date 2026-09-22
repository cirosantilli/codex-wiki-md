<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $n\ge1$. In the normalization used here, the [Dirichlet kernel](../../../../../../dirichlet-kernel.md) has the finite expansion

$$
D_j(u)=\frac12+\sum_{r=1}^j\cos(ru)
=\frac12\sum_{r=-j}^j e^{iru}.
$$

Averaging a finite number of the integral formulas for the [Fourier partial sums](../../../../../../fourier-partial-sum.md) is legitimate by linearity of the integral. Hence the [Fejér sum](../../../../../../fejer-sum.md) is [convolution](../../../../../../convolution.md) with

$$
F_n(u)=\frac1n\sum_{j=0}^{n-1}D_j(u)
=\frac12+\sum_{r=1}^{n-1}\left(1-\frac rn\right)\cos(ru).
$$

To obtain the nonnegative form of the [Fejér kernel](../../../../../../fejer-kernel.md), expand a squared geometric sum:

$$
\left|\sum_{\ell=0}^{n-1}e^{i\ell u}\right|^2
=n+2\sum_{r=1}^{n-1}(n-r)\cos(ru).
$$

The coefficient $n-r$ counts pairs of indices whose difference is $r$. Dividing by $2n$ and summing the geometric progression gives

$$
\boxed{F_n(u)=\frac1{2n}\left|\sum_{\ell=0}^{n-1}e^{i\ell u}\right|^2
=\frac1{2n}\frac{\sin^2(nu/2)}{\sin^2(u/2)}}.
$$

At $u\in2\pi\mathbb Z$ the ratio has its continuous limiting value $F_n(u)=n/2$. Thus this is a continuous, nonnegative [trigonometric polynomial](../../../../../../trigonometric-polynomial.md), not a kernel with genuine singularities.

Integration over a full period kills every nonconstant cosine term, so

$$
\int_{\mathbb T}F_n(u)\,du=\pi.
$$

Translation invariance of integration over the circle consequently gives, for every $x$,

$$
|\sigma_n(f,x)|
\le\frac1\pi\int_{\mathbb T}F_n(x-t)|f(t)|\,dt
\le\frac{\|f\|_\infty}{\pi}\int_{\mathbb T}F_n(x-t)\,dt
=\|f\|_\infty.
$$

The first step is the integral triangle inequality, the second uses nonnegativity, and the last uses the mass just computed. Taking the [supremum norm](../../../../../../supremum-norm.md) proves

$$
\boxed{\|\sigma_n(f)\|_\infty\le\|f\|_\infty}.
$$

In particular, [Fejér summation is a uniform-norm contraction](../../../../../../fejer-summation-is-a-uniform-norm-contraction.md). The factor $\pi$, rather than $2\pi$, is essential for the half-normalized [Dirichlet kernel](../../../../../../dirichlet-kernel.md) and [Fejér kernel](../../../../../../fejer-kernel.md) in this problem.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
