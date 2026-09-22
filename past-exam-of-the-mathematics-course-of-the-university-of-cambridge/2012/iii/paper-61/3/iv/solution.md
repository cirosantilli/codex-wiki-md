<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $k_y=0$ and nonzero $k_x$, the [wavenumber](../../../../../../wavenumber.md) is constant. Continuity gives $\dot{\widetilde\Sigma}'=-ik_x\Sigma_0\widetilde v_x$, and the conserved [vortensity](../../../../../../vortensity.md) relation gives

$$
ik_x\widetilde v_y=\Sigma_0\widetilde q'+\frac{(2\Omega-S)\widetilde\Sigma'}{\Sigma_0}.
$$

Differentiate continuity and substitute radial momentum and this identity. The [forced axisymmetric density mode with vortensity](../../../../../../forced-axisymmetric-density-mode-with-vortensity.md) obeys

$$
\boxed{\ddot{\widetilde\Sigma}'+\omega_k^2\widetilde\Sigma'=-2\Omega\Sigma_0^2\widetilde q',\qquad\omega_k^2=c_s^2k_x^2-2\pi G\Sigma_0|k_x|+\kappa^2,\quad\kappa^2=2\Omega(2\Omega-S).}
$$

The constant forcing represents the stationary vortical or balanced component, which is lost if every mode is assumed to have nonzero frequency. Let $k_*=\pi G\Sigma_0/c_s^2=\kappa/(Qc_s)$. Completing the square gives

$$
\omega_k^2=c_s^2(|k_x|-k_*)^2+\kappa^2(1-Q^{-2}).
$$

For $Q>1$, every nonzero radial [wavenumber](../../../../../../wavenumber.md) has positive $\omega_k^2$. The solution is a constant balanced offset $-2\Omega\Sigma_0^2\widetilde q'/\omega_k^2$ plus bounded sine and cosine oscillations. [Pressure](../../../../../../pressure.md) stabilizes short wavelengths, rotation stabilizes long wavelengths, and self-gravity is strongest at intermediate wavelengths.

For $Q<1$, the [Toomre stability criterion](../../../../../../toomre-s-stability-criterion.md) fails in the band

$$
\boxed{k_*\left(1-\sqrt{1-Q^2}\right)<|k_x|<k_*\left(1+\sqrt{1-Q^2}\right).}
$$

There $\omega_k^2<0$ and the homogeneous solutions grow or decay exponentially. The fastest rate is $s_{\max}=\kappa\sqrt{Q^{-2}-1}$ at $|k_x|=k_*$. Outside the band the modes oscillate; at its edges the frequency vanishes.

At $Q=1$, $\omega_k^2\geq0$ and it vanishes only at $|k_x|=\kappa/c_s$. At that critical [wavenumber](../../../../../../wavenumber.md),

$$
\boxed{\widetilde\Sigma'(t)=C_0+C_1t-\Omega\Sigma_0^2\widetilde q' t^2.}
$$

This [Toomre marginal algebraic growth](../../../../../../toomre-marginal-algebraic-growth.md) is spectrally marginal, not bounded for all data: a nonzero conserved [vortensity](../../../../../../vortensity.md) gives quadratic secular growth, and even zero [vortensity](../../../../../../vortensity.md) can allow the linear term. Other wavenumbers still oscillate about a balanced offset. **$Q>1$ gives bounded axisymmetric modes, $Q<1$ allows exponential instability, and $Q=1$ has a zero-frequency marginal mode with possible algebraic growth.** These statements are axisymmetric; nonaxisymmetric shearing disturbances can have transient swing behavior. For $k_x=k_y=0$, continuity instead fixes the uniform [mass density](../../../../../../density.md) shift, while the velocities execute epicyclic motion; no $1/k$ gravitational formula is used.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
