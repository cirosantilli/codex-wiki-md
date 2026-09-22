<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a vertical ray, the [transmittance](../../../../transmittance.md) from $p_2$ to space is $\mathcal T_\nu(p_2)=e^{-\tau_\nu(p_2)}$. Direct integration of the full pressure-dependent [Lorentz line shape](../../../../lorentz-line-shape.md) gives, for $d>0$,

$$
\tau_\nu(p_2)=\frac qg\int_0^{p_2}\kappa_\nu(p)\,dp
=C\ln\left[1+\left(\frac{\Delta_s p_2}{p_s d}\right)^2\right].
$$

The exact Lorentz-model [transmittance](../../../../transmittance.md) and its [strong-line limit](../../../../strong-line-limit.md) are therefore

$$
\boxed{\mathcal T_\nu(p_2)=\left[1+\left(\frac{\Delta_s p_2}{p_s d}\right)^2\right]^{-C}
\simeq\exp\left[-\left(\frac{wp_2}{p_s d}\right)^2\right].}
$$

The approximation is justified at the radiating level by $C\gg1$. At zenith-angle cosine $\mu$, replace $\tau$ by $\tau/\mu$; if a hemispheric flux transmission is desired, its normalized value is $2\int_0^1\mu e^{-\tau/\mu}d\mu=2E_3(\tau)$. The pure Lorentz model formally gives infinite line-centre [optical depth](../../../../optical-depth.md) from every nonzero $p_2$ to $p=0$, because $\kappa_{\nu_0}\propto1/p$. This is an unphysical central-core singularity, addressed in part (d), rather than a divergence of the integrated outgoing [flux](../../../../flux.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
