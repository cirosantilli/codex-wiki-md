<h1 id="b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

A [normal mode](../../../../normal-mode.md) is a motion in which all generalized coordinates oscillate at one [frequency](../../../../frequency.md) with fixed [amplitude](../../../../wave-amplitude.md) ratios. Small [oscillations](../../../../oscillation.md) about [stable equilibrium](../../../../stable-equilibrium.md) in a time-independent conservative system give $\mathsf M\ddot{\boldsymbol\theta}+\mathsf K\boldsymbol\theta=0$, with positive [mass matrix](../../../../mass-matrix.md) and symmetric [stiffness matrix](../../../../stiffness-matrix.md), allowing a generalized normal-mode eigenproblem.

For the [three-to-one mass double-pendulum modes](../../../../three-to-one-mass-double-pendulum-modes.md), the angles are absolute displacements from vertical, as printed. To quadratic order,

$$
K=\frac{m\ell^2}{2}(4\dot\theta_1^2+2\dot\theta_1\dot\theta_2+\dot\theta_2^2),\qquad
U=\frac{mg\ell}{2}(4\theta_1^2+\theta_2^2).
$$

For $\boldsymbol\theta=\mathbf A\cos\omega t$ and $q=\omega^2\ell/g$, the determinant is

$$
\det\begin{pmatrix}4-4q&-q\\-q&1-q\end{pmatrix}
=3q^2-8q+4=(3q-2)(q-2).
$$

Thus

$$
\boxed{\omega_-^2=\frac{2g}{3\ell},\quad(\theta_1,\theta_2)\propto(1,2);
\qquad\omega_+^2=\frac{2g}{\ell},\quad(\theta_1,\theta_2)\propto(1,-2).}
$$

The low [mode](../../../../mode-statistics.md) has the strings leaning together, with the lower angle twice as large; the high [mode](../../../../mode-statistics.md) has opposite angular signs. Both reverse together after half their respective periods.

For the specified release, decompose $(\alpha,\alpha)=(3\alpha/4)(1,2)+(\alpha/4)(1,-2)$. Therefore

$$
\theta_1=\frac\alpha4(3\cos\omega_-t+\cos\omega_+t),\qquad
\theta_2=\frac\alpha2(3\cos\omega_-t-\cos\omega_+t),
$$

and the lower [mass](../../../../mass.md)'s horizontal displacement is

$$
\boxed{x_m\simeq\ell(\theta_1+\theta_2)
=\frac{\alpha\ell}{4}(9\cos\omega_-t-\cos\omega_+t),\qquad
\sup|x_m|=\frac52|\alpha|\ell.}
$$

This is the [supremum of two incommensurate harmonic modes](../../../../supremum-of-two-incommensurate-harmonic-modes.md), conventionally described as the maximum-amplitude estimate. Strictly, $\omega_+/\omega_-=\sqrt3$ is irrational, so the opposite cosine extrema are approached arbitrarily closely but never coincide at a finite time. The quoted value is a [supremum](../../../../supremum.md) of the ideal linearized motion.

<a id="b6/image-original-normal-mode-motion-sketches-and-the-lower-mass-displacement-after-equal-angle-release-with-the-limiting-amplitude-bound-marked"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1-gpp2014-double-pendulum.png)

**[Figure 2](#b6/image-original-normal-mode-motion-sketches-and-the-lower-mass-displacement-after-equal-angle-release-with-the-limiting-amplitude-bound-marked). Original normal-mode motion sketches and the lower-mass displacement after equal-angle release, with the limiting amplitude bound marked**.

## ↑ Ancestors (12)

1. [B6](../b6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
