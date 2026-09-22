<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Type-I [phase matching](../../../../phase-matching.md) requires $n_{e,2\omega}(\theta)=n_{o,\omega}$, because both pump [photons](../../../../photon.md) are ordinary and the harmonic is extraordinary. Apply the direction-dependent index equation to the harmonic, not to the pump. Solving gives

$$
\sin^2\theta=
\frac{n_{o,\omega}^{-2}-n_{o,2\omega}^{-2}}
{n_{e,2\omega}^{-2}-n_{o,2\omega}^{-2}}.
$$

For the ruby-laser data this is $0.626210$, whereas the shorter-wavelength data give $0.958873$. Therefore

$$
\boxed{\theta_{694\to347}=52.31^\circ,\qquad
\theta_{515\to257.5}\simeq78.30^\circ.}
$$

The second calculation uses the supplied $257\,\mathrm{nm}$ indices as rounded harmonic data: the exact half-wavelength of $515\,\mathrm{nm}$ is $257.5\,\mathrm{nm}$. The index dispersion between those two ultraviolet values was not supplied.

For an extraordinary wave, its [Poynting vector](../../../../poynting-vector.md) makes an angle $\theta_S$ with the optic axis satisfying $\tan\theta_S=(n_o^2/n_e^2)\tan\theta$. Thus the [spatial walk-off](../../../../spatial-walk-off.md) angle relative to the [wave vector](../../../../wavevector.md) is

$$
\rho=\arctan\left(\frac{n_{o,2\omega}^2}{n_{e,2\omega}^2}\tan\theta\right)-\theta,
\qquad
\boxed{\rho_{347}=1.601^\circ,\quad\rho_{257.5}\simeq0.731^\circ.}
$$

Both angles refer to the harmonic. The ordinary pump does not have this angular walk-off. For beam radius $w_b$, the approximate overlap length is $w_b/\tan\rho$, so the shorter-wavelength geometry has about $2.19$ times the walk-off-limited interaction length.[§§2.8.2–2.8.3, printed pp. 156–158: extraordinary index and energy-flux direction](../../../../fundamentals-of-photonics-and-quantum-electronics-lecture-notes-by-franz-x-kartner.md)

To compare coupling, take propagation azimuth $\varphi$ and ordinary unit polarization $(-\sin\varphi,\cos\varphi,0)$. Its quadratic source is $P_z=-\epsilon_0d_{36}E_0^2\sin2\varphi$. Projection onto an extraordinary displacement direction with $z$ component proportional to $\sin\theta$ gives $|d_{\rm eff}|\propto|d_{36}\sin\theta\sin2\varphi|$, up to the small anisotropic normalization correction. The optimal azimuth is $45^\circ$. At equal beam area, interaction length, input power and approximately equal nonlinear coefficients, the shorter pump has both stronger angular coupling and the favorable frequency-squared factor:

$$
\frac{\eta_{515}}{\eta_{694}}\simeq
\left(\frac{694}{515}\right)^2
\frac{\sin^2\theta_{515}}{\sin^2\theta_{694}}
\frac{n_{o,694}^3}{n_{o,515}^3}\simeq2.73.
$$

Here $\eta=P_{2\omega}/P_\omega$ in the small-conversion, equal-area model, with harmonic index phase-matched to the pump. Its smaller [spatial walk-off](../../../../spatial-walk-off.md) further favors the $515\,\mathrm{nm}$ pump in a walk-off-limited geometry. **Equal input power alone does not determine an absolute efficiency ranking**: ultraviolet absorption, wavelength-dependent $d_{36}$, beam size, crystal length and coatings are unspecified. For example, a sufficiently strongly absorbing $257.5\,\mathrm{nm}$ output can reverse the ideal ranking. The stated preference is conditional on comparable transparent crystals and comparable focusing, not a prediction independent of those parameters.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
