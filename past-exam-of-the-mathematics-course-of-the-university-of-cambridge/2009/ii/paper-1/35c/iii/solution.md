<h1 id="35c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use signature $(-,+,+,+)$, for which $\Box=-\partial_t^2+\Delta$. With the [Lorenz constraint in Proca theory](../../../../../../lorenz-constraint-in-proca-theory.md), the [Proca equation](../../../../../../proca-equation.md) is $(\Box-m^2)A^a=-\mu_0J^a$. A static solution therefore satisfies $(\Delta-m^2)A^a=-\mu_0J^a$.

For $R>0$ direct radial differentiation gives $(\Delta-m^2)(e^{-mR}/R)=0$. At the origin its $1/R$ singularity contributes $-4\pi\delta_0$: integrating the Laplacian over a small sphere gives limiting outward flux $-4\pi$, while the mass term's integral tends to zero. Thus $G_m(R)=e^{-mR}/(4\pi R)$ obeys $(\Delta-m^2)G_m=-\delta_0$. Convolution proves the printed [Yukawa potential](../../../../../../yukawa-potential.md) solution

$$
\boxed{A^a(x)=\frac{\mu_0}{4\pi}\int\frac{e^{-m|x-x'|}}{|x-x'|}J^a(x')\,d^3x'.}
$$

The integral requires suitable source decay, for example compact support. For conserved static sources, differentiating the convolution and integrating by parts gives $\partial_aA^a=0$ as well; its spatial divergence is the convolution with $\partial_iJ^i=0$.

For the usual nonnegative mass parameter this is the decaying static solution, and $m=0$ gives the Coulomb kernel with Lorenz gauge imposed. If the arbitrary real parameter is negative, the printed kernel still gives a particular solution for compact sources, but grows at infinity; the decaying boundary condition selects $e^{-|m|R}/(4\pi R)$ instead. Static sources also allow homogeneous time-dependent solutions, so this construction establishes a static solution, not that every solution is static.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [35C](../../35c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
