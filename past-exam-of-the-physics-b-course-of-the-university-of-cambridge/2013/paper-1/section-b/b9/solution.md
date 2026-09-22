<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For cold, collisionless, unmagnetized electrons with stationary heavy ions, $-m_e\omega^2\mathbf x=-e\mathbf E$. Therefore $\mathbf P=-ne\mathbf x=-ne^2\mathbf E/(m_e\omega^2)$ and

$$
\boxed{\epsilon_r(\omega)=1-\frac{\omega_p^2}{\omega^2},\qquad
\omega_p=\sqrt{\frac{ne^2}{m_e\epsilon_0}}.}
$$

This is the [cold collisionless plasma dielectric response](../../../../../cold-collisionless-plasma-dielectric-response.md). For a propagating transverse wave, $\mathbf B=\mathbf k\times\mathbf E/\omega$, so $E/B=c$ in vacuum and $E/B=c/n_p$ in [plasma](../../../../../plasma-physics.md), where $n_p=\sqrt{\epsilon_r}$. Equivalently $E/H=Z_0$ and $Z_0/n_p$ for $\mu=\mu_0$.

Converting the [density](../../../../../density.md) gives $n=10^{18}\,\mathrm{m^{-3}}$, so $\omega_p=5.64\times10^{10}\,\mathrm{s^{-1}}$ and $f_p=8.98\,\mathrm{GHz}$. At $10\,\mathrm{GHz}$,

$$
\boxed{\epsilon_r\simeq0.19384,\qquad n_p\simeq0.4403.}
$$

At an interface without independently imposed surface charge or sheet current, tangential $\mathbf E,\mathbf H$ and normal $\mathbf B,\mathbf D$ are continuous, with the electron response included in the effective [permittivity](../../../../../permittivity-split.md). Normal $E$ need not be continuous; the induced electron charge is represented by that response. In a convention treating it explicitly as a surface charge, the normal vacuum-displacement jump equals that charge instead.

For the downward transmitted wave, transversality gives $k_xE_x+k_zE_z=0$. The measured field therefore has $k_x/(-k_z)=3$, so $\tan\theta_t=3$ and $\sin\theta_t=3/\sqrt{10}$. Tangential [phase matching](../../../../../phase-matching.md) gives

$$
\boxed{\theta_i=\sin^{-1}\left(n_p\frac3{\sqrt{10}}\right)\simeq24.69^\circ.}
$$

For [inferring incident power from a transmitted plasma field](../../../../../inferring-incident-power-from-a-transmitted-plasma-field.md), choose $\mathbf E_i=E_i(\cos\theta_i,0,\sin\theta_i)$ and $\mathbf E_r=E_r(\cos\theta_i,0,-\sin\theta_i)$. Their [magnetic fields](../../../../../magnetic-field-split.md) have opposite $y$ directions. The two tangential conditions are

$$
(E_i+E_r)\cos\theta_i=1\,\mathrm{V\,m^{-1}},\qquad
E_i-E_r=n_p\sqrt{10}\,\mathrm{V\,m^{-1}}.
$$

Hence $E_i\simeq1.2464\,\mathrm{V\,m^{-1}}$ and $E_r\simeq-0.1458\,\mathrm{V\,m^{-1}}$. Since these are peak phasor amplitudes,

$$
\boxed{\langle S_i\rangle=\frac{E_i^2}{2Z_0}
\simeq2.06\times10^{-3}\,\mathrm{W\,m^{-2}}.}
$$

This is incident [power](../../../../../power.md) per area perpendicular to its propagation. Per area of the interface the incoming normal flux is $\langle S_i\rangle\cos\theta_i\simeq1.87\times10^{-3}\,\mathrm{W\,m^{-2}}$. The reflected sign is a phase reversal, not negative reflected [energy](../../../../../energy-split.md).

At $1\,\mathrm{GHz}<f_p$, the [relative permittivity](../../../../../relative-permittivity.md) is negative and there is no propagating transverse bulk wave. The field decays evanescently into the [plasma](../../../../../plasma-physics.md) and the ideal collisionless half-space reflects all incoming normal [power](../../../../../power.md). Collisions would allow absorption; a [complex refractive index](../../../../../complex-refractive-index.md) here does not by itself imply dissipative heating.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
