<h1 id="1/b/waveform-dilation">Waveform dilation</h1>

↑ **Parent:** [Solution](solution.md)

For $b>0$, put $\psi_b(z,t)=\psi(bz,bt)$. Each derivative gains a factor $b$, so $\mathcal L_b(z,t)=b^2\mathcal L(bz,bt)$. Changing integration variables to $(Z,T)=(bz,bt)$ contributes $b^{-2}$, proving exact invariance of the full-space [action](../../../../action.md).

Set $b=1+\eta$. At fixed coordinates, $\delta\psi=\eta X$ with $X=z\psi'+t\dot\psi$. Since the density is quadratic in derivatives,

$$
\frac{\delta\mathcal L}{\eta}=2\mathcal L+z\partial_z\mathcal L+t\partial_t\mathcal L
=\partial_t(t\mathcal L)+\partial_z(z\mathcal L).
$$

The variation is a divergence, so subtract its boundary term in the [Noether current](../../../../noether-current.md):

$$
j_2^0=\Pi X-t\mathcal L=t\mathcal H+z\Pi\psi',\qquad
j_2^z=-AK\psi'X-z\mathcal L=-tAK\dot\psi\psi'-z\mathcal H.
$$

Thus the [dilatation charge of a one-dimensional elastic wave](../../../../dilatation-charge-of-a-one-dimensional-elastic-wave.md) is

$$
\boxed{Q_2=\int_{-\infty}^{\infty}\left(t\mathcal H+z\Pi\psi'\right)dz}.
$$

An overall sign change would give the same [conservation law](../../../../conservation-law.md). Unlike $Q_1$, this charge has units of [action](../../../../action.md), $\mathrm{J\,s}$. Its explicit factor of $t$ is balanced by transport of the weighted [momentum](../../../../momentum-split.md) density; an explicitly time-dependent charge can still be conserved.

## ↑ Ancestors (15)

1. [Solution](solution.md)
2. [B](../b.md)
3. [1](../../1.md)
4. [2017](../../../2017-split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../list-of-universities.md)
15. [Codex Wiki](../../../../split.md)
