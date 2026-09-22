<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $r=r_0+\eta$, where $|\eta|\ll r_0$. The [Taylor expansion](../../../../taylor-expansion.md) at a [circular orbit](../../../../circular-orbit.md) is

$$
V_{\mathrm{eff}}(r_0+\eta)=V_{\mathrm{eff}}(r_0)
+\frac12V_{\mathrm{eff}}''(r_0)\eta^2+O(\eta^3).
$$

The constant $V_{\mathrm{eff}}(r_0)$ has no effect on the [force](../../../../force-split.md). The paper's displayed [harmonic potential](../../../../harmonic-potential.md) should be read as this expansion after subtracting that constant and neglecting higher orders; it is not an equality for the absolute [effective potential](../../../../effective-potential.md) in general. For example, when $m=J=\beta=1$ and $k=2$, $r_0=2^{-1/4}$ and $V_{\mathrm{eff}}(r_0)=\sqrt2$, whereas the printed quadratic expression is zero at $r_0$.

Differentiating again and then using $\beta k r_0^{k-2}=J^2/(mr_0^4)$ gives

$$
\begin{aligned}
V_{\mathrm{eff}}''(r_0)&=\beta k(k-1)r_0^{k-2}+\frac{3J^2}{mr_0^4}\\
&=(k+2)\frac{J^2}{mr_0^4}.
\end{aligned}
$$

The linearized radial [equation of motion](../../../../equation-of-motion.md) is $m\ddot\eta=-V_{\mathrm{eff}}''(r_0)\eta$, so the [radial frequency in a power-law central potential](../../../../radial-frequency-in-a-power-law-central-potential.md) is

$$
\boxed{\omega_r=\sqrt{k+2}\,\frac{|J|}{mr_0^2},\qquad k>-2.}
$$

For $k<-2$ the [circular orbit](../../../../circular-orbit.md) is unstable and radial disturbances grow exponentially, with growth rate $\sqrt{-(k+2)}|J|/(mr_0^2)$. At $k=-2$ the linear restoring [force](../../../../force-split.md) vanishes, as described in part (c). Thus an attractive [central force](../../../../central-force.md) alone does not guarantee [small oscillations](../../../../small-oscillation.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
