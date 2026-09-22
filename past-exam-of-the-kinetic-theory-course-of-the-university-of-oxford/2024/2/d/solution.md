<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $\kappa=|k|$ and first work with a representative positive $k=\kappa$. For $\kappa\lambda_{\mathrm{De}}\ll1$, the thermal core is strongly screened. However, the causal [dielectric function](../../../../dielectric-function.md) has weakly damped [Langmuir wave](../../../../langmuir-wave.md) roots $\omega_s+i\gamma_s$, with $s=\pm1$, $\omega_s\simeq s\omega_{pe}$ and $\gamma_s<0$. Their [phase velocities](../../../../phase-velocity.md) $v_s=\omega_s/\kappa$ are in the tail. Both roots must be retained for each spatial [Fourier series](../../../../fourier-series-split.md) harmonic.

Write $\epsilon(-i\omega+0^+,\kappa)=\epsilon_R(\omega)+i\epsilon_I(\omega)$. The supplied approximation gives

$$
\epsilon_R\simeq1-\frac{\omega_{pe}^2}{\omega^2},\qquad \epsilon_I\simeq-\frac{\pi\omega_{pe}^2}{\kappa^2n_e}f_0'(\omega/\kappa),\qquad \epsilon_R'(\omega_s)\simeq\frac2{\omega_s}.
$$

Expanding $\epsilon(\omega_s+i\gamma_s)=0$ to first order gives the [Landau damping](../../../../landau-damping.md) rate

$$
\gamma_s=-\frac{\epsilon_I(\omega_s)}{\epsilon_R'(\omega_s)}\simeq\frac{\pi\omega_s\omega_{pe}^2}{2\kappa^2n_e}f_0'(v_s).
$$

In particular, stable damping means $\omega_sf_0'(v_s)<0$. Near either root,

$$
|\epsilon(-i\kappa v+0^+,\kappa)|^2\simeq\frac4{\omega_{pe}^2}\left[(\kappa v-\omega_s)^2+\gamma_s^2\right].
$$

The narrow [Lorentzian resonance approximation](../../../../lorentzian-resonance-approximation.md) then gives the leading resonant contribution

$$
\frac1{|\epsilon(-i\kappa v+0^+,\kappa)|^2}\simeq\frac{\pi\omega_{pe}^2}{4}\sum_{s=\pm1}\frac{\delta(\kappa v-\omega_s)}{|\gamma_s|}.
$$

This is a formula under the [integral](../../../../integral-split.md) over [velocity](../../../../velocity.md); it is not a pointwise approximation away from the [resonances](../../../../resonance.md). Insert it into the heating formula in [c](../c.md). For one spatial harmonic, the contribution from one root is

$$
\begin{aligned}
Q_{k,s}
&=-\frac{e^2}{m_e}k^2A_k\frac{\pi\omega_{pe}^2}{4\kappa}\frac{v_sf_0'(v_s)}{|\gamma_s|}\\
&=\frac{e^2n_e}{2m_e}k^2A_k,
\end{aligned}
$$

because

$$
\frac{v_sf_0'(v_s)}{|\gamma_s|}=-\frac{2\kappa n_e}{\pi\omega_{pe}^2}.
$$

Thus the tiny tail slope cancels the tiny [Landau damping](../../../../landau-damping.md) rate: weak absorption is compensated by a large noise-driven wave intensity. The two temporal roots supply two equal halves of the answer. Negative $k$ gives the same result by the conjugate response of a real [electric field](../../../../electric-field-split.md), without altering the original convention that the spatial sum includes both signs. Therefore

$$
\boxed{\frac{d\mathcal K}{dt}=\sum_k\sum_{s=\pm1}Q_{k,s}\simeq\frac{e^2n_e}{m_e}\sum_k k^2A_k.}
$$

As in [c](../c.md), equality means the leading result in the stated asymptotic limit. This calculation assumes nonzero damping, observation times $t\gg\max_s|\gamma_s|^{-1}$, and forcing weak enough that $f_0$ changes negligibly during that relaxation. Taking zero damping before the long-time limit invalidates the stationary calculation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
