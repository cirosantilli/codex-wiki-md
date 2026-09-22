<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the steady periodic response, the cycle average of the [mechanical energy](../../../../mechanical-energy.md) derivative vanishes. The applied [average power](../../../../average-power.md) therefore equals the power dissipated by the viscous [force](../../../../force-split.md):

$$
\overline P=m\gamma\langle\dot z^{\,2}\rangle=\frac12m\gamma A^2\omega^2.
$$

Using [solution](../b/solution.md) gives

$$
\boxed{\overline P(\omega)=\frac{F_0^2m\gamma\omega^2}{2\big[(k-m\omega^2)^2+(m\gamma\omega)^2\big]}.}
$$

The same result follows from averaging the instantaneous input [power](../../../../power.md) $F(t)\dot z(t)$, using the response [phase](../../../../phase-waves.md) relative to the drive.

For positive $m,k,\gamma$ and $\omega>0$, rewrite this as

$$
\overline P=\frac{F_0^2}{2m\gamma}\,
\frac{(m\gamma\omega)^2}{(k-m\omega^2)^2+(m\gamma\omega)^2}.
$$

The last factor is at most one, with equality precisely when $k-m\omega^2=0$. Thus the power peak occurs at $\omega_0=\sqrt{k/m}$ and

$$
\boxed{\overline P_{\max}=\frac{F_0^2}{2m\gamma}.}
$$

This power-resonance [angular frequency](../../../../angular-frequency.md) is exactly $\omega_0$; it need not equal the [angular frequency](../../../../angular-frequency.md) maximizing displacement [amplitude](../../../../wave-amplitude.md). Positive damping is essential: at $\gamma=0$ and exact resonance there is no bounded steady periodic response to nonzero forcing, so the divergent expression is not a finite-power solution.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
