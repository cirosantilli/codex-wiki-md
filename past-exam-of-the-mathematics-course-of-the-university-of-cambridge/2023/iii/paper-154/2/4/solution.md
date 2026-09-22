<h1 id="2/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The displayed estimate requires the standard choice $\psi(r)=r$; read literally, the printed $\psi'(r)=r$ would give $\psi=r^2/2$, $-\Delta^2\psi=0$, and would not imply the claimed estimate. For $\psi=|x|$, the [distributional bilaplacian of the radial coordinate in three dimensions](../../../../../../distributional-bilaplacian-of-the-radial-coordinate-in-three-dimensions.md) is

$$
-\Delta^2\psi=8\pi\delta_0,
\qquad
\Delta\psi=\frac2r,
\qquad
\psi''=0.
$$

The delta term is nonnegative. The Morawetz action is bounded by $CE$ using Cauchy-Schwarz and the [Hardy inequality in Euclidean space](../../../../../../hardy-inequality-in-euclidean-space.md). Integrating the identity from $0$ to $T$ and discarding the delta term gives

$$
\int_0^T\int_{\mathbb R^3}\frac{|u|^{p+1}}{|x|}\,dx\,dt
\leq CE(u(0)),
$$

uniformly in $T$, proving the [Morawetz estimate for the defocusing wave equation](../../../../../../morawetz-estimate-for-the-defocusing-wave-equation.md).

A finite-energy stationary solution would make the nonnegative spatial integral on the left constant in time. Its integral over $[0,\infty)$ can be finite only when that spatial integral is zero, so the stationary solution is $u=0$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2](../../2.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
