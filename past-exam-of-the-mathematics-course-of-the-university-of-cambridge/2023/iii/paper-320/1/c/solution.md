<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The sudden potential change leaves the star's position and velocity unchanged. Its new energy is therefore

$$
E_1=E_0+\frac{G(M_0-M_1)}r
=-\frac{GM_0}{2a}+\frac{GM_0}{2r}
=\frac{GM_0}{2}\left(\frac1r-\frac1a\right).
$$

Thus $E_1>0$ precisely when $r<a$. Parametrize the orbit by [eccentric anomaly](../../../../../../eccentric-anomaly.md) $\eta$:

$$
r=a(1-e\cos\eta),
\qquad
\theta_r=\eta-e\sin\eta.
$$

A [phase-mixed orbit](../../../../../../phase-mixed-orbit.md) is uniform in the [mean anomaly](../../../../../../mean-anomaly.md) $\theta_r$. For $e>0$, the condition $r<a$ is $-\pi/2<\eta<\pi/2$ modulo one period. The corresponding mean-anomaly interval has length

$$
\Delta\theta_r
=\left[\eta-e\sin\eta\right]_{-\pi/2}^{\pi/2}
=\pi-2e.
$$

Hence

$$
\boxed{P_{\rm unbound}(e)=\frac12-\frac e\pi}.
$$

The energy increase $G(M_0-M_1)/r$ is largest near [periapsis](../../../../../../periapsis.md), so stars are more readily unbound there than near [apoapsis](../../../../../../apoapsis.md). A perfectly circular orbit is the measure-zero marginal case $E_1=0$ at every phase.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
