<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In deep [radiation domination](../../../../../../radiation-domination.md), $a\propto\tau$ and $a'/a=1/\tau$. Neglect $\Omega_c\delta_c$ against the radiation gravity source, so the supplied [CDM density equation in a matter-radiation universe](../../../../../../cdm-density-equation-in-a-matter-radiation-universe.md) becomes

$$
\delta_c''+\frac1\tau\delta_c'=\frac3{\tau^2}\delta_r.
$$

On [superhorizon scales](../../../../../../superhorizon-scale.md) omit the $k^2\delta_r/3$ pressure-gradient term. Under [adiabatic initial conditions](../../../../../../adiabatic-initial-conditions.md), $\delta_r=(4/3)\delta_c$ then gives

$$
\delta_c''+\frac1\tau\delta_c'-\frac4{\tau^2}\delta_c=0.
$$

The [Euler-Cauchy equation](../../../../../../euler-cauchy-equation.md) characteristic polynomial is $p^2-4$, so

$$
\boxed{\delta_c=A_r(\mathbf k)(\tau/\tau_i)^2+
B_r(\mathbf k)(\tau/\tau_i)^{-2},
\qquad \delta_r=\frac43\delta_c.}
$$

These are the general growing and decaying adiabatic solutions in this approximation. A regular primordial growing mode discards the divergent $\tau^{-2}$ solution. Although its conformal-time growth is again quadratic, now $\delta_c\propto a^2$, rather than $\delta_c\propto a$ in [matter domination](../../../../../../matter-domination.md).

If “general” is taken without imposing adiabaticity, both independent relative-entropy integration constants must also be retained. The gradient-free radiation equation gives

$$
S=\delta_r-\frac43\delta_c=S_0+S_1\tau.
$$

Substitution into the matter equation produces

$$
\delta_c=C_g\tau^2+C_d\tau^{-2}-\frac34S_0-S_1\tau,\qquad
\delta_r=\frac43C_g\tau^2+\frac43C_d\tau^{-2}-\frac13S_1\tau.
$$

This is the general solution of the leading supplied coupled system, described by the [superhorizon radiation-era entropy integration constants](../../../../../../superhorizon-radiation-era-entropy-integration-constants.md). Setting both $S_0$ and $S_1$ to zero recovers the adiabatic result. Regularity and the full initial [Einstein field equations](../../../../../../einstein-field-equations.md) constraints can further restrict which of these leading solutions represents a prescribed physical initial mode.

On scales well inside the horizon, radiation pressure drives oscillations at frequency approximately $k/\sqrt3$. Their amplitude is bounded at leading order, and their gravitational forcing of a slowly varying matter contrast can be averaged away. With this approximation, as well as negligible matter self-gravity,

$$
\delta_c''+\frac1\tau\delta_c'\simeq0,\qquad
(\tau\delta_c')'\simeq0,
$$

hence the [logarithmic CDM growth after radiation-era horizon entry](../../../../../../logarithmic-cdm-growth-after-radiation-era-horizon-entry.md) is

$$
\boxed{\delta_c=C_0(\mathbf k)+C_{\log}(\mathbf k)
\log(\tau/\tau_h),\qquad k\tau\gg1,\quad\tau\ll\tau_{\rm eq}.}
$$

This is the [Mészáros effect](../../../../../../meszaros-effect.md). It does not mean that $\delta_r$ itself vanishes. For a rapidly oscillating source $R_\gamma\cos(\omega\tau+\varphi)$, the matter equation has a particular response

$$
\delta_{c,\rm osc}\simeq
-\frac{3R_\gamma}{\omega^2\tau^2}\cos(\omega\tau+\varphi).
$$

Its leading second derivative reproduces $3\delta_r/\tau^2$; the remaining terms are smaller by powers of $(k\tau)^{-1}$. Thus the [suppressed cold-matter forcing by rapid radiation oscillations](../../../../../../suppressed-cold-matter-forcing-by-rapid-radiation-oscillations.md) is only order $\delta_r/(k\tau)^2$ and does not change the secular logarithm. Radiation forcing near horizon entry determines $C_0,C_{\log}$ and cannot be averaged away there. Neither this smoothing approximation nor the neglect of matter gravity remains uniformly valid near equality.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
