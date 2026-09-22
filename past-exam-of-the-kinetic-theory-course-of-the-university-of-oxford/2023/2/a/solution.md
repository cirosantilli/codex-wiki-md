<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The step in the source must be at zero.** We use the [Heaviside step function](../../../../heaviside-step-function.md) $H(x)=1$ for $x>0$, zero for $x<0$, with its value at zero immaterial here. The printed threshold $1$ is inconsistent with both $H'=\delta(x)$ and the stated [number density](../../../../number-density.md). For example, measuring [velocities](../../../../velocity.md) in fixed units and taking $v_F=2$, the literal printed cutoff fills only $v<1$ and gives one eighth of the stated [number density](../../../../number-density.md). Its [distributional derivative](../../../../distributional-derivative.md) is $\delta(x-1)$, not $\delta(x)$. The zero-threshold convention restores the stated [Fermi sphere](../../../../fermi-sphere.md) and its [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md).

Let $k=|\mathbf k|>0$, choose $u=\mathbf v\cdot\mathbf k/k$, and abbreviate $V_\alpha=v_{\mathrm F\alpha}$. The three-dimensional [phase-space distribution function](../../../../phase-space-distribution-function.md) is $f_{0\alpha}=C_\alpha\mathbf1_{v<V_\alpha}$, where

$$
C_\alpha=\frac{m_\alpha^3}{4\pi^3\hbar^3}=\frac{3n_\alpha}{4\pi V_\alpha^3}.
$$

Integrate over the transverse [velocity](../../../../velocity.md) disk to obtain the parallel [marginal distribution](../../../../marginal-distribution.md)

$$
F_\alpha(u)=\int f_{0\alpha}\,d^2v_\perp
=\frac{3n_\alpha}{4V_\alpha^3}(V_\alpha^2-u^2)\mathbf1_{|u|<V_\alpha},\qquad
F_\alpha'(u)=-\frac{3n_\alpha u}{2V_\alpha^3}\mathbf1_{|u|<V_\alpha}.
$$

There are no edge [Dirac delta functions](../../../../dirac-delta-function.md) in $F_\alpha'$ because $F_\alpha$ itself vanishes continuously at the endpoints. In particular, the three-dimensional constant occupation does not imply a constant parallel [marginal distribution](../../../../marginal-distribution.md).

Use time dependence $e^{pt+i\mathbf k\cdot\mathbf x}$, with $p=\gamma-i\omega$ and $\gamma<0$ for [damping](../../../../damping.md). The given [dielectric function](../../../../dielectric-function.md) becomes

$$
\epsilon=1-\sum_\alpha\frac{\omega_{\mathrm p\alpha}^2}{n_\alpha k^2}
\int_{C_L}\frac{F_\alpha'(u)}{u-\omega/k-i\gamma/k}\,du.
$$

The [Landau contour](../../../../landau-contour.md) supplies causal continuation. For a real [phase velocity](../../../../phase-velocity.md) $a=\omega/k>V_\alpha$, there is no resonant pole in the populated interval, and

$$
\begin{aligned}
\int\frac{F_\alpha'(u)}{u-a}\,du
&=-\frac{3n_\alpha}{2V_\alpha^3}\int_{-V_\alpha}^{V_\alpha}\frac{u}{u-a}\,du\\
&=-\frac{3n_\alpha}{2V_\alpha^3}\left[2V_\alpha+a\log\frac{a-V_\alpha}{a+V_\alpha}\right].
\end{aligned}
$$

Hence this species contributes

$$
\chi_\alpha=\frac{3\omega_{\mathrm p\alpha}^2}{k^2V_\alpha^2}
\left[1+\frac{s_\alpha}{2}\log\frac{s_\alpha-1}{s_\alpha+1}\right],\qquad
s_\alpha=\frac{\omega}{kV_\alpha}>1.
$$

For comparable species [number densities](../../../../number-density.md) and fixed charge ratios, $m_e\ll m_i$ implies $V_i/V_e=O(m_e/m_i)$ and $\omega_{\mathrm pi}^2/\omega_{\mathrm pe}^2=O(m_e/m_i)$. Since $\omega>kV_e$, the ions have $s_i\gg1$ and $\chi_i=-\omega_{\mathrm pi}^2/\omega^2+O(k^2V_i^2\omega_{\mathrm pi}^2/\omega^4)$. Their response is negligible to leading order in the [mass](../../../../mass.md) ratio. The real [dispersion relation](../../../../dispersion-relation-split.md) is therefore

$$
\boxed{1+\frac{3\omega_{\mathrm pe}^2}{k^2V_e^2}\left[1+\frac{\omega}{2kV_e}\log\frac{\omega-kV_e}{\omega+kV_e}\right]=0.}
$$

This [degenerate-plasma dielectric response](../../../../degenerate-plasma-dielectric-response.md) treats a completely degenerate, nonrelativistic [Fermi gas](../../../../fermi-gas.md) with classical particle trajectories. It does not include quantum recoil or a collision term. A finite ion response shifts the root slightly; the boxed equation is the stated leading electron approximation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
