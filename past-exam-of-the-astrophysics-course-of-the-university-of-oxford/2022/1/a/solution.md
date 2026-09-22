<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [specific intensity](../../../../spectral-radiance.md) $I_\nu$ is [energy](../../../../energy-split.md) transported per unit time, projected area, [solid angle](../../../../solid-angle.md) and [frequency](../../../../frequency.md). The path coordinate $s$ increases along the ray. The [emission coefficient](../../../../emission-coefficient.md) $j_\nu$ is emitted [energy](../../../../energy-split.md) per unit time, volume, [solid angle](../../../../solid-angle.md) and [frequency](../../../../frequency.md), whereas the [absorption coefficient](../../../../absorption-coefficient.md) $\alpha_\nu$ has units of inverse length. Thus $j_\nu ds$ adds [specific intensity](../../../../spectral-radiance.md) and $\alpha_\nu I_\nu ds$ removes it. [Stimulated emission](../../../../stimulated-emission.md) can be included as negative [absorption](../../../../absorption-electromagnetic-radiation.md).

Define the [optical depth](../../../../optical-depth.md) between two points by $\tau_\nu(s_1,s_2)=\int_{s_1}^{s_2}\alpha_\nu(u)\,du$. Multiplying the [radiative transfer equation](../../../../radiative-transfer-equation.md) by the [integrating factor](../../../../integrating-factor.md) $\exp[\tau_\nu(s_0,s)]$ and integrating gives

$$
\boxed{I_\nu(s)=I_\nu(s_0)e^{-\tau_\nu(s_0,s)}+\int_{s_0}^{s}j_\nu(u)e^{-\tau_\nu(u,s)}\,du.}
$$

Each local contribution is attenuated only by the material between its emission point and the observer. Where $\alpha_\nu\ne0$, the [source function](../../../../radiative-transfer-source-function.md) is $S_\nu=j_\nu/\alpha_\nu$ and the same [formal solution of the radiative transfer equation](../../../../formal-solution-of-the-radiative-transfer-equation.md) is $I_\nu(\tau)=I_\nu(0)e^{-\tau}+\int_0^\tau S_\nu(t)e^{-(\tau-t)}dt$. A constant [source function](../../../../radiative-transfer-source-function.md) gives $I_\nu=I_\nu(0)e^{-\tau}+S_\nu(1-e^{-\tau})$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
