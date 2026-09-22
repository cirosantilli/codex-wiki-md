<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider a narrow bundle of rays between two surface elements $dA_1,dA_2$ separated by $s$ in a transparent, stationary Euclidean vacuum. Let the ray make angles $\theta_1,\theta_2$ to the respective surface normals. The receiving element subtends [solid angle](../../../../../../solid-angle.md) $d\Omega_1=\cos\theta_2dA_2/s^2$ at the emitter. By the definition of [specific intensity](../../../../../../specific-intensity.md), the beam power in frequency interval $d\nu$ is

$$
d\mathcal P_\nu=I_{\nu,1}\cos\theta_1dA_1\,d\Omega_1\,d\nu
=I_{\nu,1}\frac{\cos\theta_1\cos\theta_2dA_1dA_2}{s^2}\,d\nu.
$$

At the receiving end the source subtends $d\Omega_2=\cos\theta_1dA_1/s^2$, so the identical power is

$$
d\mathcal P_\nu=I_{\nu,2}\frac{\cos\theta_1\cos\theta_2dA_1dA_2}{s^2}\,d\nu.
$$

In the absence of absorption, emission or frequency shifts, [conservation of energy](../../../../../../conservation-of-energy.md) equates these expressions:

$$
\boxed{I_{\nu,2}=I_{\nu,1}.}
$$

This [vacuum conservation of specific intensity](../../../../../../vacuum-conservation-of-specific-intensity.md) also follows directly from the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) $dI_\nu/ds=0$. The apparent [solid angle](../../../../../../solid-angle.md) of an unresolved source shrinks as $s^{-2}$, so its integrated observed [radiative flux](../../../../../../radiative-flux.md) still follows the inverse-square law. Specific intensity and unresolved flux are different quantities.

The vacuum and frequency assumptions are essential: absorption and emission change [specific intensity](../../../../../../specific-intensity.md), and gravitational or cosmological redshift conserves $I_\nu/\nu^3$ along a ray instead of $I_\nu$ itself. A fixed telescope aperture observing an unresolved object also cannot infer constant total received power from intensity conservation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
