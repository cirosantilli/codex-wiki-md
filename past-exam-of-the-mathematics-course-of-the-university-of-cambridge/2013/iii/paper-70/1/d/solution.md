<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\alpha=\Omega\tau_0^*$ and $s=\sin\theta$, where $\tau_0^*=t-R/c_0$. Label the two arms by $\sigma=\pm1$. Their positions are $y_\sigma=\sigma r e_r(\Omega\tau_\sigma^*)$. To radiating far-field accuracy,

$$
|x-y_\sigma|=R-\sigma rs\cos(\Omega\tau_\sigma^*)+O(a^2/R).
$$

The [retarded time](../../../../../../retarded-time.md) equation therefore gives, with $\mu_r=\Omega r/c_0$,

$$
\Omega\tau_\sigma^*=\alpha+\sigma\mu_rs\cos(\Omega\tau_\sigma^*)+O(\Omega a^2/(c_0R))
=\alpha+\sigma\mu_rs\cos\alpha+O(\mu^2,\Omega a^2/(c_0R)).
$$

For the first arm, $\sigma=1$, this is the requested phase expansion. The more explicit geometric error also makes the dimensional meaning of the printed $O(1/R)$ term clear.

Apply the [Taylor theorem](../../../../../../taylor-theorem.md) to the rotating line [force](../../../../../../force.md). Since $de_\phi/d\alpha=-e_r$, its first two orders, expressed in a common reference frame, are

$$
F_\sigma(r,\tau_\sigma^*)=\frac{2r}{a^2}
\left[F\sigma e_\phi(\alpha)+D e_x-F\mu_rs\cos\alpha\,e_r(\alpha)\right]+O\left(\frac{r}{a^2}|F|\mu^2\right).
$$

Also $v_\sigma=\sigma\Omega r e_\phi(\Omega\tau_\sigma^*)$, so the [radial Mach number](../../../../../../radial-mach-number.md) is

$$
M_{r,\sigma}=-\sigma\mu_rs\sin\alpha+O(\mu^2),\qquad
\boxed{|1-M_{r,\sigma}|^{-1}=1-\sigma\mu_rs\sin\alpha+O(\mu^2).}
$$

The absolute value causes no change of sign in this subsonic limit. Multiplying these two expansions before summing is essential: both the shifted [force](../../../../../../force.md) and the [moving-surface retarded Jacobian](../../../../../../moving-surface-retarded-jacobian.md) contribute at the same order.

Denote the integrated numerator, including that Jacobian, by $\mathcal B$. Pairing the two blades cancels all terms odd in $\sigma$, including the first Doppler correction to the axial load. Hence

$$
\begin{aligned}
\mathcal B(\alpha,n)
&=\sum_{\sigma=\pm1}\int_0^a\frac{F_\sigma(r,\tau_\sigma^*)}{1-M_{r,\sigma}}\,dr\\
&=2D e_x-\frac{4F\Omega a}{3c_0}s\left(\cos\alpha\,e_r(\alpha)+\sin\alpha\,e_\phi(\alpha)\right)+O\big((|F|+|D|)\mu^2\big)\\
&=2D e_x-\frac{4F\Omega a}{3c_0}s\left(\cos2\alpha\,e_y+\sin2\alpha\,e_z\right)+O\big((|F|+|D|)\mu^2\big).
\end{aligned}
$$

The factor $a/3$ comes from $a^{-2}\int_0^a r^2dr$. Only the time-dependent term radiates at order $R^{-1}$. Applying $-\partial_{x_i}$ to the integral now gives $\rho'_{\rm rad}=(4\pi c_0^3R)^{-1}n\cdot\partial_t\mathcal B$, and thus

$$
\boxed{\rho'_{\rm rad}=\frac{2F\Omega^2a}{3\pi c_0^4R}\sin^2\theta\,
\sin\big(2\Omega(t-R/c_0)\big)+O\left(\frac{(|F|+|D|)\Omega\mu^2}{c_0^3R}\right).}
$$

There are also nonradiating terms of order $R^{-2}$. Multiply by $c_0^2$ for the acoustic [pressure](../../../../../../pressure.md). The stated coefficient uses the rotation convention fixed above; reversing the rotation reverses the corresponding signed load and phase convention.

This is a [compact rotating two-blade loading source](../../../../../../compact-rotating-two-blade-loading-source.md) acting as an [acoustic quadrupole](../../../../../../acoustic-quadrupole.md). The compact total rotating [force](../../../../../../force.md) cancels, leaving the first spatial moment of the loading. Its two factors of the observer's projection into the rotor plane produce $\sin^2\theta$: there is no leading sound on the rotation axis and the density amplitude is maximal in the rotor plane. The configuration repeats after half a rotation, explaining frequency $2\Omega$. These statements concern amplitude; the corresponding [acoustic intensity](../../../../../../acoustic-energy-flux.md) has a $\sin^4\theta$ factor.

If $F=0$, the displayed first-order contribution vanishes as well. For completeness, expanding the axial Jacobian to its next even order gives

$$
(1-M_{r,\sigma})^{-1}=1-\sigma\mu_rs\sin\alpha-\mu_r^2s^2\cos2\alpha+O(\mu_r^3).
$$

The first remaining axial-load radiation is then

$$
\rho'_{D,\rm rad}=\frac{D\Omega^3a^2}{2\pi c_0^5R}\cos\theta\sin^2\theta\sin2\alpha+\text{higher orders}.
$$

Thus the constant axial total [force](../../../../../../force.md) does not produce the lower-order term, even though its moving spatial distribution can radiate at a higher order.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
