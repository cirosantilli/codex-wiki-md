<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $\gamma>0$, the [positive diffusivity requirement for the forward heat kernel](../../../../../../../positive-diffusivity-requirement-for-the-forward-heat-kernel.md). A [normal mode](../../../../../../../normal-mode.md) $e^{ikx-i\omega t}$ of the [linear complex Ginzburg-Landau equation](../../../../../../../linear-complex-ginzburg-landau-equation.md) gives

$$
D(k,\omega)=-i\omega+iUk-\mu+\gamma k^2=0,\qquad
\omega(k)=Uk+i(\mu-\gamma k^2).
$$

For real $k$, the maximum [temporal growth rate](../../../../../../../growth-rate.md) is $\mu$. The [Briggs-Bers criterion](../../../../../../../briggs-bers-criterion.md) starts the inverse time [Laplace transform](../../../../../../../laplace-transform.md) above the temporal growth spectrum and follows the two spatial roots as its frequency contour is lowered. A contributing [spatial pinch point](../../../../../../../spatial-pinch-point.md) occurs when roots continued from opposite sides of the spatial contour coalesce and prevent its deformation. An arbitrary algebraic saddle is not sufficient without this branch selection.

Here $D=D_k=0$ gives

$$
\boxed{k_0=-\frac{iU}{2\gamma},\qquad
\omega_0=i\left(\mu-\frac{U^2}{4\gamma}\right)}.
$$

To check the pinch, start at $\omega=i\Omega$ with $\Omega$ large. The roots are $k=-iU/(2\gamma)\pm i\sqrt{U^2+4\gamma(\Omega-\mu)}/(2\gamma)$ and initially lie in opposite half-planes. They meet at $\Omega=\mu-U^2/(4\gamma)$, giving the causal saddle. Positive imaginary [absolute frequency](../../../../../../../absolute-frequency.md) means fixed-position exponential growth. Therefore

$$
\boxed{\text{absolute hydrodynamic instability: }\mu>\frac{U^2}{4\gamma}},\qquad
\boxed{\text{convective hydrodynamic instability: }0<\mu<\frac{U^2}{4\gamma}}.
$$

For $\mu\le0$ there is no positive temporal growth. At $\mu=U^2/(4\gamma)$ the fixed-position exponential rate is zero; its algebraic prefactor, derived below, decays. When $U=0$ the convective interval is empty.

The source specifies only real coefficients. For $\gamma<0$, temporal growth is unbounded at high real [wavenumber](../../../../../../../wavenumber.md), so the usual causal forward-diffusion construction is ill posed and the above criterion does not apply. For $\gamma=0$ the equation reduces to transport with amplification; its point impulse remains a moving delta, rather than a spreading [heat kernel](../../../../../../../heat-kernel.md). These cases cannot be included by division by $\gamma$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
