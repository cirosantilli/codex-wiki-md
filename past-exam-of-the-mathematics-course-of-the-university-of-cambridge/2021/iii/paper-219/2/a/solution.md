<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The squared chord distance is

$$
\lVert u(t)-u(t')\rVert^2
=2-2\cos\{\omega(t-t')\}
=4\sin^2\left(\frac{\omega(t-t')}{2}\right).
$$

Hence the restricted [Gaussian process](../../../../../../gaussian-process.md) has covariance

$$
\boxed{
k_\theta(t,t')
=A\exp\left[-\frac{2}{l^2}
\sin^2\left\{\frac{\omega(t-t')}{2}\right\}\right]}.
$$

It depends only on $t-t'$, so it is stationary. It is periodic in either argument with period $T=2\pi/\omega$, and Gaussian-process realizations inherit that period almost surely because $f(t+T)-f(t)$ has zero variance.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
