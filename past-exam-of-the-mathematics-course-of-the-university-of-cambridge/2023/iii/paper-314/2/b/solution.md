<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $Y=B_\phi^2$, $x=R^2/L^2$, and retain the frozen axial field $B_z=(B_0/\rho_0)\rho$. The radial [magnetostatic equilibrium](../../../../../../magnetostatic-equilibrium.md) equation now includes both the gradient of the toroidal [magnetic pressure](../../../../../../magnetic-pressure.md) and the inward [magnetic tension](../../../../../../magnetic-tension.md):

$$
\frac d{dR}(K_{\rm eff}\rho^2)
+\rho\Phi'
+\frac{Y'}{8\pi}
+\frac{Y}{4\pi R}=0.
$$

For $\rho=\rho_1e^{-x}$, cylindrical gravity gives

$$
\Phi'(R)=\frac{2G\lambda(<R)}R
=\frac{2\pi G\rho_1L^2}{R}(1-e^{-x}).
$$

Multiplication by the [integrating factor](../../../../../../integrating-factor.md) $R^2$ therefore produces

$$
\frac d{dR}(R^2Y)
=-8\pi R^2\left[\rho\Phi'+\frac d{dR}(K_{\rm eff}\rho^2)\right].
$$

The integration constant must vanish for regularity on the axis. Direct integration gives

$$
\boxed{
B_\phi^2(R)=\frac{4\pi\rho_1^2}{R^2}
\left\{
K_{\rm eff}L^2[1-(1+2x)e^{-2x}]
-\pi GL^4(1-e^{-x})^2
\right\}}.
$$

Its [Taylor expansion](../../../../../../taylor-expansion.md) at the axis is

$$
B_\phi^2
=4\pi\rho_1^2(2K_{\rm eff}-\pi GL^2)\frac{R^2}{L^2}
+O(R^4),
$$

so the regular field behaves as $B_\phi=O(R)$. At large radius,

$$
B_\phi^2\sim
\frac{4\pi\rho_1^2L^2}{R^2}(K_{\rm eff}-\pi GL^2).
$$

Nonnegativity at infinity requires

$$
\boxed{L^2\leq\frac{K_{\rm eff}}{\pi G}}.
$$

This condition is also sufficient: at the limiting value, the braces divided by $K_{\rm eff}L^2$ reduce to $2e^{-x}[1-(1+x)e^{-x}]\geq0$, and decreasing $L^2$ only increases them. Thus the [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) is real and regular at every radius exactly in the stated range.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
