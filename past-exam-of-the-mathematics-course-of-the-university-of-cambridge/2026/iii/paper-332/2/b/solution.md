<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The diffusion length suggests the [similarity variable](../../../../../../similarity-variable.md)

$$
\eta=\frac{z}{2\sqrt{\kappa t}},
\qquad
h(t)=2\lambda\sqrt{\kappa t}.
$$

The [Neumann solution of the Stefan problem](../../../../../../neumann-solution-of-the-stefan-problem.md), written using the [error function](../../../../../../error-function.md), is

$$
\boxed{
T_i(z,t)=T_b+(T_m-T_b)
\frac{\operatorname{erf}\eta}{\operatorname{erf}\lambda}},
$$



$$
\boxed{
T_w(z,t)=T_\infty+(T_m-T_\infty)
\frac{\operatorname{erfc}\eta}{\operatorname{erfc}\lambda}}.
$$

These expressions satisfy all four thermal [boundary conditions](../../../../../../boundary-condition.md). At the interface,

$$
T_{i,z}
=\frac{T_m-T_b}{\sqrt{\pi\kappa t}}
\frac{e^{-\lambda^2}}{\operatorname{erf}\lambda},
\qquad
T_{w,z}
=\frac{T_\infty-T_m}{\sqrt{\pi\kappa t}}
\frac{e^{-\lambda^2}}{\operatorname{erfc}\lambda}.
$$

Since $\dot h=\lambda\sqrt{\kappa/t}$ and $k=\rho c_p\kappa$, the [Stefan condition](../../../../../../stefan-condition.md) becomes

$$
\boxed{
\frac{L}{c_p}\sqrt{\pi}\lambda e^{\lambda^2}
=\frac{T_m-T_b}{\operatorname{erf}\lambda}
-\frac{T_\infty-T_m}{\operatorname{erfc}\lambda}}.
$$

The second term represents heat supplied from the warm water and therefore reduces the freezing rate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
