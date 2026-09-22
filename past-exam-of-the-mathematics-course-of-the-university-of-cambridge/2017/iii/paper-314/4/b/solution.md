<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The separation of the two bodies is $a$, as is fixed by the supplied [Kepler third law](../../../../../../kepler-s-third-law.md) $\omega_o^2=G(M_1+M_2)/a^3$. The phrase “orbit of radius $a$” cannot denote the first body's distance from the center of mass in that formula.

Expand the companion's [Newtonian potential of a point mass](../../../../../../newtonian-potential-of-a-point-mass.md) about the first body's center. The constant term produces no force; the linear term produces the uniform acceleration of the center and disappears in the translating frame. The leading differential acceleration therefore comes from the [quadrupolar tidal forcing](../../../../../../quadrupolar-tidal-forcing.md)

$$
\Phi_{\mathrm{tide}}=-\frac{GM_2}{2a^3}\left[3(\mathbf n(t)\cdot\mathbf r)^2-r^2\right],
$$

where $\mathbf n(t)$ points toward the companion. It is a degree-two solid [spherical harmonic](../../../../../../spherical-harmonic.md). For a circular nonrotating-frame orbit, its time-dependent components have $m=\pm2$ and frequency $2\omega_o$, because the squared direction cosines repeat twice per orbit. There is also a static $m=0$ component. The real part of one complex harmonic represents the pair of time-dependent components; its normalization and orientation are absorbed into the order-one coefficient $\psi$. This gives $\Psi=\psi(GM_2/a^3)r^2Y_2^m$ and $\omega=2\omega_o$. The expansion is the leading term for $R_1/a$ small; spin is being neglected.

For a forced [potential flow](../../../../../../potential-flow.md) with the same temporal frequency, the [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) becomes

$$
-\omega^2\nabla U=-\nabla\left(\frac{\delta p}{\rho_1}+\delta\Phi+\Psi\right).
$$

Use $U=A r^2Y_2^m$. The [surface gravity perturbation of a uniform-density sphere](../../../../../../surface-gravity-perturbation-of-a-uniform-density-sphere.md) is unchanged, as is the vanishing [Lagrangian pressure perturbation](../../../../../../lagrangian-pressure-perturbation.md) boundary condition. Integrating the equation and applying that condition gives

$$
(\omega^2-\omega_2^2)A=\psi\frac{GM_2}{a^3},\qquad
\omega_2^2=\frac45\frac{GM_1}{R_1^3}.
$$

Since $\xi_r(R_1)=2AR_1Y_2^m$, the real surface [displacement](../../../../../../displacement.md) is

$$
\boxed{\xi_r(R_1,t)=\epsilon R_1\frac{\omega_2^2}{\omega^2-\omega_2^2}
\operatorname{Re}\!\left(\psi Y_2^m e^{-i\omega t}\right),\qquad
\epsilon=\frac52\frac{M_2}{M_1}\left(\frac{R_1}{a}\right)^3.}
$$

Indeed $\epsilon\omega_2^2=2GM_2/a^3$, so the normalization is consistent. This is a particular forced response away from the [resonance](../../../../../../resonance.md); arbitrary free [normal modes](../../../../../../normal-mode.md) can be added.

Put $\mu=M_2/M_1$ and $q=(R_1/a)^3$. The [tidal resonance of a stellar oscillation](../../../../../../tidal-resonance-of-a-stellar-oscillation.md) condition is $4\omega_o^2=\omega_2^2$, hence

$$
q=\frac1{5(1+\mu)},\qquad
\epsilon=\frac{\mu}{2(1+\mu)},\qquad
\boxed{\left(\frac{R_1}{a}\right)^3=\frac15(1-2\epsilon).}
$$

The resonance gives $0\leq\epsilon<1/2$ for finite nonnegative $\mu$, with actual forcing requiring $M_2>0$. At exact [resonance](../../../../../../resonance.md) the undamped [linearization](../../../../../../linearization.md) has no bounded response at the forcing frequency: the time-domain particular solution grows proportionally to $t$ times a sinusoid. Thus the frequency-response formula has a pole, rather than describing a finite resonant [displacement](../../../../../../displacement.md). Away from that pole, [linearization](../../../../../../linearization.md) requires the displayed surface displacement to be small compared with $R_1$; the leading [quadrupolar tidal forcing](../../../../../../quadrupolar-tidal-forcing.md) approximation separately requires $R_1/a$ small.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
