<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the positive-[frequency](../../../../frequency.md) branch write $s=1+\delta$, $\delta>0$, and $Q=k^2V_e^2/(3\omega_{\mathrm pe}^2)=\kappa^2/3$. The [degenerate-plasma dielectric response](../../../../degenerate-plasma-dielectric-response.md) is equivalent to

$$
1+\frac{1+\delta}{2}\log\frac{\delta}{2+\delta}=-Q.
$$

At large $Q$, a logarithmic divergence is needed to balance the right-hand side; hence $\delta\ll1$. Keeping the constant as well as the large term gives

$$
\log\frac\delta2=-2(1+Q)+O(\delta|\log\delta|),\qquad
\boxed{\delta\sim2\exp\left[-2-\frac{2k^2V_e^2}{3\omega_{\mathrm pe}^2}\right].}
$$

More precisely the relative correction is $O((1+Q)e^{-2(1+Q)})$. The additive constant $-2$ in the exponent fixes the leading prefactor $2e^{-2}$ and should not be discarded.

The negative-[frequency](../../../../frequency.md) branch follows from the even real [dielectric function](../../../../dielectric-function.md) outside the occupied interval. Thus

$$
\boxed{\omega_\pm=\pm kV_e(1+\delta),\qquad
\delta\sim2\exp\left[-2-\frac29(k\lambda_{\mathrm De}^{\rm exam})^2\right].}
$$

Using the physical [Thomas-Fermi screening length](../../../../thomas-fermi-screening-length.md) instead gives $\delta\sim2e^{-2-2(k\lambda_{\rm TF})^2}$. This is [degenerate-plasma zero-point sound](../../../../degenerate-plasma-zero-point-sound.md): the [phase velocity](../../../../phase-velocity.md) lies exponentially close to, but strictly beyond, the edge of the [Fermi sphere](../../../../fermi-sphere.md) for every finite $k$ in this approximation. The limit is a property of the supplied classical-trajectory [kinetic theory](../../../../kinetic-theory-split.md); applying it at microscopic [wavelengths](../../../../wavelength.md) would require checking quantum recoil, which that equation omits.

## ↑ Ancestors (12)

1. [D](../d.md)
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
