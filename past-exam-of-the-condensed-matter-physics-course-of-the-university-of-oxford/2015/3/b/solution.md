<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u_p$ be the longitudinal displacement of atom $p$. Translational invariance and a symmetric harmonic pair force give the [long-range harmonic-chain dispersion](../../../../long-range-harmonic-chain-dispersion.md) equations

$$
M\ddot u_p=\sum_{n\ne0}C_{|n|}(u_{p+n}-u_p)
=\sum_{n>0}C_n(u_{p+n}+u_{p-n}-2u_p).
$$

Use a traveling [normal mode](../../../../normal-mode.md) $u_p=u_0e^{i(kpa-\omega t)}$. Dividing by its nonzero amplitude gives

$$
-M\omega^2=\sum_{n>0}C_n(e^{inka}+e^{-inka}-2)
=-4\sum_{n>0}C_n\sin^2(nka/2).
$$

Hence

$$
\boxed{\omega(k)=\frac2{\sqrt M}\left[\sum_{n>0}C_n\sin^2(nka/2)\right]^{1/2}}.
$$

Positive pair constants give a nonnegative squared [frequency](../../../../frequency.md) and a uniform-translation zero mode. More general signed force constants require checking stability of the entire sum. The [frequency](../../../../frequency.md) is even in $k$ and periodic with $2\pi/a$, reflecting reciprocal-lattice equivalence. The force sum must converge in the model. A finite ordinary acoustic slope additionally requires convergence of $\sum n^2C_n$, in which case $v_s=a\sqrt{\sum n^2C_n/M}$. Both finite-range examples below satisfy this condition.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
