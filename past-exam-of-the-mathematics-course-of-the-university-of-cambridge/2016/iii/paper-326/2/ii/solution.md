<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [maximum-entropy regularization functional](../../../../../../maximum-entropy-regularization-functional.md), differentiation of the scalar integrand gives $(s\log s-s)'=\log s$. Thus the [Fréchet derivative](../../../../../../frechet-derivative.md) at a positive reference function $y$ is $E'(y)=\log y$, and the stated differentiability result gives $\partial E(y)=\{\log y\}$. Consequently,

$$
\boxed{D_E(x,y)=\int_\Omega\left[x\log\frac{x}{y}-x+y\right]dt.}
$$

This is the [generalized Kullback–Leibler divergence](../../../../../../generalized-kullback-leibler-divergence.md). When both functions integrate to the same mass, the last two terms cancel after integration; for [probability density functions](../../../../../../probability-density-function.md) it becomes the usual [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md). For two positive functions, adding the reverse distance gives

$$
\boxed{D_E^{\mathrm{sym}}(x,y)=\int_\Omega(x-y)(\log x-\log y)\,dt.}
$$

A sufficient setting for the differentiability argument is $L^\infty(\Omega)$ with $y$ bounded away from zero. For nonnegative $x$, use $0\log(0/y)=0$ wherever appropriate. Positivity alone in $L^2$ does not automatically provide an open domain on which the [Fréchet derivative](../../../../../../frechet-derivative.md) exists.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
