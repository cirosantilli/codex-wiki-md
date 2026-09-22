<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The nonconstant exponential modes of the leading basin equation satisfy

$$
\nu\lambda^3-r\lambda-\beta=0.
$$

Thus a leading uniformly valid form is $\bar\psi\simeq S(y)x/\beta+C_0(y)+\sum_{j=1}^3C_j(y)e^{\lambda_jx}$, with exponentials referenced to the wall where they decay. The coefficients enforce the four east/west no-slip conditions; their values are not needed to identify the scales.

If $r^3\ll\beta^2\nu$, horizontal viscosity dominates drag in the [boundary layers](../../../../../../boundary-layer.md). The [Munk boundary layer](../../../../../../munk-boundary-layer.md) scale is $\delta_M=(\nu/\beta)^{1/3}$, assumed much smaller than basin width. The roots are $\delta_M^{-1}$ and $(-1\pm i\sqrt3)/(2\delta_M)$ to leading order, so

$$
\boxed{\bar\psi\simeq\frac{S(y)}\beta x+C_0(y)+A(y)e^{(x-1)/\delta_M}
+e^{-x/(2\delta_M)}\left[B(y)\cos\frac{\sqrt3x}{2\delta_M}+C(y)\sin\frac{\sqrt3x}{2\delta_M}\right].}
$$

The east layer has exponential thickness $\delta_M$ and the west oscillatory layer has envelope thickness $2\delta_M$, both of order $\delta_M$. The west correction supplies the order-one return transport, while the east no-slip correction is typically smaller in amplitude. Setting $r=0$ still leaves enough viscous modes to impose no-slip.

If $r^3\gg\beta^2\nu$, linear drag dominates the broad vorticity layer. Define

$$
\delta_S=\frac r\beta,\qquad \delta_v=\sqrt{\frac\nu r},\qquad
\frac{\delta_v}{\delta_S}=\left(\frac{\beta^2\nu}{r^3}\right)^{1/2}\ll1,
$$

with $\delta_S$ small compared with basin width. The roots are approximately $-\delta_S^{-1}$ and $\pm\delta_v^{-1}$; the fast roots have smaller correction $\beta/(2r)$. The [drag-dominated basin solution with no-slip layers](../../../../../../drag-dominated-basin-solution-with-no-slip-layers.md) is

$$
\boxed{\bar\psi\simeq\frac{S(y)}\beta x+C_0(y)+A(y)e^{-x/\delta_S}
+B(y)e^{-x/\delta_v}+C(y)e^{(x-1)/\delta_v}.}
$$

There is a broad western [Stommel boundary layer](../../../../../../stommel-boundary-layer.md) of thickness $\delta_S$, a thinner western no-slip layer of thickness $\delta_v$, and an eastern no-slip layer of thickness $\delta_v$. The narrow layers can have small [streamfunction](../../../../../../stream-function.md) amplitude while supplying an order-one change in wall velocity.

If viscosity is set identically to zero, only the particular solution, a constant and the western Stommel exponential remain. That second-order model cannot generally satisfy both [streamfunction](../../../../../../stream-function.md) and derivative conditions at both walls. **Small nonzero viscosity must be retained in the wall skins when no-slip is required.** In the question's stress notation, the limits compare $[\gamma/(\rho_0H)]^3$ with $\beta^2\nu$. Neither limit applies at the crossover, where all cubic terms contribute. These composite forms are leading asymptotic solutions of the basin problem; meridional derivatives and interior diffusion supply higher-order corrections.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
