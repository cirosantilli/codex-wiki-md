<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When $m_1=m_2=\mu^2$, the [free energy](../../../../../../thermodynamic-free-energy.md) has [continuous symmetry](../../../../../../continuous-symmetry.md) $O(2)$. Its ordered minima satisfy

$$
\rho_0^2=\phi_1^2+\phi_2^2=-\frac{\mu^2}{4g}.
$$

Continuous phase fluctuations make the lower critical dimension $d_{\rm l}=2$, in agreement with the [Mermin-Wagner theorem](../../../../../../mermin-wagner-theorem.md). In two dimensions write the complex [order parameter](../../../../../../order-parameter.md) as $\psi=\rho_0e^{i\theta}$. Neglecting the massive [amplitude mode](../../../../../../higgs-mode.md) gives the [Goldstone-mode effective free energy](../../../../../../goldstone-mode-effective-free-energy.md)

$$
F_\theta=\frac{\rho_0^2}{2}\int d^2x\,(\nabla\theta)^2.
$$

The [phase-difference variance](../../../../../../phase-difference-variance.md) is

$$
\langle[\theta(x)-\theta(0)]^2\rangle
=\frac1{\pi\rho_0^2}\log\frac r a+O(1),
$$

and therefore

$$
\langle\psi(x)\psi(0)^*\rangle
\sim \rho_0^2\exp\left[-\frac12
\langle(\theta(x)-\theta(0))^2\rangle\right]
\sim r^{-\eta},
$$

with

$$
\boxed{\eta=\frac1{2\pi\rho_0^2}=-\frac{2g}{\pi\mu^2}.}
$$

Thus [spin waves](../../../../../../spin-wave.md) replace true long-range order by [quasi-long-range order](../../../../../../quasi-long-range-order.md).

A [vortex](../../../../../../phase-vortex.md)-antivortex pair of separation $R$ has the logarithmic energy $E_{\rm pair}\simeq2\pi\rho_0^2\log(R/a)$. The number of pair separations below $R$ grows as $R^2$, giving the coarse entropy $S_{\rm pair}\simeq2\log(R/a)$. Thus

$$
F_{\rm pair}\simeq2(\pi\rho_0^2-1)\log(R/a),
$$

and widely separated pairs become favorable at $\rho_0^2\simeq1/\pi$. Substituting the mean-field stiffness gives

$$
\boxed{\mu^2\simeq-\frac{4g}{\pi},}
$$

suggesting a [Berezinskii–Kosterlitz–Thouless transition](../../../../../../berezinskii-kosterlitz-thouless-transition.md). The numerical location is only a bare-stiffness estimate: vortex-core fluctuations renormalize the stiffness near the transition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
