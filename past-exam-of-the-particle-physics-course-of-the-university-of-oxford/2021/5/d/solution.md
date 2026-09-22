<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For two [photons](../../../../photon.md), [four-momentum conservation](../../../../four-momentum-conservation.md) and their vanishing rest [masses](../../../../mass.md) give the [diphoton invariant mass](../../../../diphoton-invariant-mass.md)

$$
M^2=2E_1E_2(1-\cos\alpha).
$$

Taking a logarithmic differential,

$$
2\frac{dM}{M}=\frac{dE_1}{E_1}+\frac{dE_2}{E_2}+\frac{\sin\alpha}{1-\cos\alpha}\,d\alpha.
$$

For small mutually independent measurement errors, [propagation of uncertainty](../../../../propagation-of-uncertainty.md) consequently gives

$$
\boxed{\left(\frac{\sigma_M}{M}\right)^2=\frac14\left[\left(\frac{\sigma_{E_1}}{E_1}\right)^2+\left(\frac{\sigma_{E_2}}{E_2}\right)^2+\left(\frac{\sin\alpha\,\sigma_\alpha}{1-\cos\alpha}\right)^2\right].}
$$

**Printed-formula correction.** The source's left-hand side, if it means $(\Delta M/M)^2$ as its description suggests, is missing the factor $1/4$ on the right. Its right-hand side instead equals $\operatorname{Var}(M^2)/M^4$ to first order. A concrete counterexample is a fixed opening angle and an exactly known $E_2$: because $M\propto\sqrt{E_1}$, a small $1\%$ fractional error in $E_1$ produces a $0.5\%$ fractional error in $M$, not $1\%$. Likewise, interpreting $\Delta M^2$ literally as a small change in $M^2$ would make the unsquared left-hand side incompatible with the squared terms. Correlated errors require the covariance terms as well.

The space angle is determined by the two polar angles and azimuthal separation:

$$
\cos\alpha=\cos\theta_1\cos\theta_2+\sin\theta_1\sin\theta_2\cos(\Delta\phi).
$$

At $\theta_1=\theta_2=45^\circ$ and $\Delta\phi=180^\circ$, $\cos\alpha=0$ and $\alpha=90^\circ$. The angular coefficient is therefore one. Equal contribution of opening-angle uncertainty and the _combined_ two independent $1\%$ [photon energy](../../../../photon-energy.md) errors requires

$$
\sigma_\alpha^2=2(0.01)^2,\qquad
\boxed{\sigma_\alpha=0.01414\ \mathrm{rad}\simeq0.81^\circ.}
$$

For independent equally precise single-[photon](../../../../photon.md) polar directions, $\sigma_\alpha^2=\sigma_{\theta_1}^2+\sigma_{\theta_2}^2$ at this geometry, so

$$
\boxed{\sigma_\theta=0.0100\ \mathrm{rad}\simeq0.57^\circ\quad\text{per photon}.}
$$

An azimuthal error contributes only at second order about $\Delta\phi=\pi$. The corresponding [invariant-mass resolution](../../../../invariant-mass-resolution.md) from the two [energy](../../../../energy-split.md) errors alone is $0.707\%$; with an equally large angular contribution it is $1.00\%$. The common missing factor of four cancels when equating the two contributions, so the angular estimates remain valid despite the printed error.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
