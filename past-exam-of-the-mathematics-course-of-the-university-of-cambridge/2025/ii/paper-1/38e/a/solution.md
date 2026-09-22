<h1 id="38e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $f(r)=1+r^2/a^2$. The geodesic [Lagrangian](../../../../../../lagrangian.md) is

$$
L=\frac12\left[-f\dot t^2+f^{-1}\dot r^2+r^2\dot\theta^2+r^2\sin^2\theta\dot\phi^2\right].
$$

Its $\theta$ equation is

$$
\frac d{d\tau}(r^2\dot\theta)-r^2\sin\theta\cos\theta\dot\phi^2=0.
$$

Spherical symmetry lets us rotate the conserved angular-momentum plane into $\theta=\pi/2$. Equivalently, initial data $\theta=\pi/2$, $\dot\theta=0$ solve this equation for all $\tau$.

The cyclic coordinates give

$$
E=f\dot t,\qquad h=r^2\dot\phi.
$$

Using the timelike normalization $g_{\mu\nu}\dot x^\mu\dot x^\nu=-1$ gives

$$
\dot r^2+f\left(1+\frac{h^2}{r^2}\right)=E^2.
$$

After separating the constant terms,

$$
\boxed{
\frac12\dot r^2+V(r)=\frac12\left(E^2-1-\frac{h^2}{a^2}\right),
\qquad
V(r)=\frac12\left(\frac{r^2}{a^2}+\frac{h^2}{r^2}\right).
}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38E](../../38e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
