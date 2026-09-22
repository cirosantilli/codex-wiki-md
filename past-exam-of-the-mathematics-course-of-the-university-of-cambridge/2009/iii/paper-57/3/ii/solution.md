<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An initially [adiabatic cosmological perturbation](../../../../../../adiabatic-initial-conditions.md) leaves the local photon-to-baryon number ratio unchanged. Since radiation density scales as the fourth power of temperature and nonrelativistic particle number as the third, its [density contrasts](../../../../../../density-contrast.md) obey $\delta_b=3\delta_\gamma/4$. With the corrected common-velocity continuity equations,

$$
\left(\delta_b-\tfrac34\delta_\gamma\right)'=k^2(\theta_b-\theta_\gamma)\simeq0,
$$

so the adiabatic relation persists in [tight coupling](../../../../../../tight-coupling-approximation.md).

Use the paper's ratio $R=4\bar\rho_\gamma/(3\bar\rho_b)$, which is the reciprocal of the commonly used [baryon loading parameter](../../../../../../baryon-loading-parameter.md). Multiply the photon Euler equation by $R$ and add the baryon Euler equation. The collision forces cancel exactly:

$$
R\theta_\gamma'+\theta_b'
=-R(\tfrac14\delta_\gamma-\sigma_\gamma)-\mathcal H\theta_b-c_{sb}^2\delta_b.
$$

This cancellation works even with the common erroneous $k^{-2}$ in the printed forces, but a physical collision rate uses the repaired forces in part (i). At leading tight-coupling order put $\theta_\gamma=\theta_b=\theta$ and substitute $\delta_b=3\delta_\gamma/4$. Then

$$
\boxed{\begin{aligned}
\delta_\gamma'&=\frac43k^2\theta,\\
\theta'&=-\frac{R}{1+R}(\tfrac14\delta_\gamma-\sigma_\gamma)
-\frac1{1+R}(\mathcal H\theta+\tfrac34c_{sb}^2\delta_\gamma).
\end{aligned}}
$$

Define the pressure-to-inertia sound speed, neglecting the very small baryon thermal pressure, by

$$
\boxed{c_s^2=\frac{R}{3(1+R)}=\frac1{3(1+3\bar\rho_b/(4\bar\rho_\gamma))}.}
$$

The combined velocity equation consequently becomes

$$
\boxed{\theta'=-3c_s^2(\tfrac14\delta_\gamma-\sigma_\gamma)
-\frac{3c_s^2}{R}(\mathcal H\theta+\tfrac34c_{sb}^2\delta_\gamma).}
$$

This is the requested [photon-baryon acoustic oscillator](../../../../../../photon-baryon-acoustic-oscillator.md) system. Photon pressure supplies the restoring force, while both photon enthalpy and baryon mass supply inertia. The retained $c_{sb}^2$ term adds the small thermal-baryon correction rather than being part of the quoted leading $c_s^2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
