<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Time and horizontal translational invariance at the interface conserve $\omega$ and $k$. For every component, horizontal momentum gives

$$
p=\frac{\rho_0(0)\omega}{k}u.
$$

The background density has the same value on both sides, so pressure continuity implies **continuity of horizontal velocity**. Normal velocity is also continuous: no fluid accumulates at the interface.

Use the particle-displacement amplitudes and polarization directions defined in part (a). For downward incident and transmitted waves and an upward reflected wave, continuity of $u$ and $w$ gives

$$
\sin\theta_1(\eta_i+\eta_r)=\sin\theta_2\eta_t,
\qquad
\cos\theta_1(\eta_i-\eta_r)=\cos\theta_2\eta_t.
$$

Solving the two equations proves the [internal-wave transmission across a buoyancy-frequency jump](../../../../../../internal-wave-transmission-across-a-buoyancy-frequency-jump.md) formula

$$
\boxed{\frac{\eta_r}{\eta_i}
=\frac{\sin\theta_2/\sin\theta_1-\cos\theta_2/\cos\theta_1}
{\sin\theta_2/\sin\theta_1+\cos\theta_2/\cos\theta_1},
\qquad
\frac{\eta_t}{\eta_i}=\frac{2\sin\theta_1\cos\theta_1}{\sin(\theta_1+\theta_2)}.}
$$

The reflected wave has the same frequency and wavelength as the incident wave and opposite vertical wavenumber. The transmitted wave has

$$
\boxed{\omega_t=\omega_i,\quad k_t=k_i,\quad
m_t=k_i\tan\theta_2,\quad\lambda_t=\lambda_i\frac{N_1}{N_2},\quad
k_i=\frac{2\pi\cos\theta_1}{\lambda_i}.}
$$

Its group velocity is downward at angle $\theta_2$; the formula in part (a), with $N_2,m_t$, gives its speed.

If instead one uses signed vertical-displacement amplitudes, the reflected coefficient has the opposite sign: $(m_1-m_2)/(m_1+m_2)$. This follows because the reflected polarization's vertical component changes sign, and is not a difference in the physical reflected field. As an energy check, the reflected fraction is $[(m_1-m_2)/(m_1+m_2)]^2$ and the transmitted fraction is $4m_1m_2/(m_1+m_2)^2$; they sum to one.

When $N_2<\omega<N_1$, take $m_t=-i\kappa$, $\kappa=k\sqrt{1-N_2^2/\omega^2}$, so $e^{im_tz}$ decays as $z\to-\infty$. The transmitted field is evanescent, carries no mean vertical energy flux, and the reflected wave has unit amplitude magnitude. A real lower-layer ray angle and wavelength are then inapplicable.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
