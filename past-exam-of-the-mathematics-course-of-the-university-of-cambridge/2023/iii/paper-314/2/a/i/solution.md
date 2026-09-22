<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The collapse is perpendicular to the initial field, so [magnetic flux freezing](../../../../../../../magnetic-flux-freezing.md) preserves the [mass-to-flux ratio](../../../../../../../mass-to-flux-ratio.md) of each material flux tube:

$$
\frac{B_z}{\rho}=\frac{B_0}{\rho_0},
\qquad
B_z=\frac{B_0}{\rho_0}\rho.
$$

With no toroidal field, radial [magnetostatic equilibrium](../../../../../../../magnetostatic-equilibrium.md) is

$$
\frac d{dR}\left(P+\frac{B_z^2}{8\pi}\right)
=-\rho\frac{d\Phi}{dR}.
$$

Define the effective polytropic constant

$$
K_{m eff}=K+\frac{B_0^2}{8\pi\rho_0^2}.
$$

Then gas and [magnetic pressure](../../../../../../../magnetic-pressure.md) combine as $P+B_z^2/(8\pi)=K_{\rm eff}\rho^2$. Dividing equilibrium by $\rho$, differentiating, and using the cylindrical [Poisson equation](../../../../../../../poisson-equation.md)

$$
\frac1R\frac d{dR}\left(R\frac{d\Phi}{dR}\right)=4\pi G\rho
$$

gives

$$
\boxed{
\frac1R\frac d{dR}\left(R\frac{d\rho}{dR}\right)
+\frac{2\pi G}{K_{\rm eff}}\rho=0}.
$$

Put $a^2=K_{\rm eff}/(2\pi G)$. This is the order-zero [Bessel differential equation](../../../../../../../bessel-differential-equation.md), and regularity on the axis together with $\rho(0)=\rho_1$ yields

$$
\boxed{\rho(R)=\rho_1J_0(R/a)}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 314](../../../../paper-314-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
