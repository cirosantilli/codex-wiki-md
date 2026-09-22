<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Ryu–Takayanagi formula](../../../../../../ryu-takayanagi-formula.md) gives the leading entropy of a static boundary region:

$$
S(D_1)=\frac{\operatorname{Area}(\gamma_{D_1})}{4G}.
$$

On the $t=0$ slice of Poincaré $\operatorname{AdS}_4$,

$$
ds^2=\frac{dz^2+d\rho^2+\rho^2d\theta^2}{z^2}.
$$

The [minimal surface](../../../../../../minimal-surface.md) anchored on a boundary circle of radius $R_1$ is the hemisphere

$$
z^2+\rho^2=R_1^2.
$$

Cutting it off at $z=\epsilon$, its area is

$$
\begin{aligned}
A_\epsilon
&=2\pi R_1\int_0^{\sqrt{R_1^2-\epsilon^2}}
\frac{\rho\,d\rho}{(R_1^2-\rho^2)^{3/2}}\\
&=2\pi\left(\frac{R_1}{\epsilon}-1\right).
\end{aligned}
$$

Therefore

$$
\boxed{
S(D_1)=\frac{\pi R_1}{2G\epsilon}
-\frac{\pi}{2G}}.
$$

The universal requirement was the perimeter-law divergence $\pi R_1/(2G\epsilon)$; the finite constant depends on the stated pure $\operatorname{AdS}_4$ vacuum geometry and equals $-\pi/(2G)$ here. Since $G\sim N^{-3/2}$, both terms are of order $N^{3/2}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 354](../../../paper-354-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
