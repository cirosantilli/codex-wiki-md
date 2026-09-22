<h1 id="section-c/c9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At low [temperature](../../../../../../temperature-split.md), $T\ll\theta_r$, retain the ground level and the first excited level. Their [energies](../../../../../../energy-split.md) are $0$ and $\hbar^2/I$, with degeneracies $1$ and $3$. Therefore

$$
Z_{\rm rot}=1+3e^{-\hbar^2/(Ik_BT)}+O\left(e^{-3\hbar^2/(Ik_BT)}\right),
$$

so in the notation of the question,

$$
\boxed{A=3,\qquad B=\frac{\hbar^2}{Ik_B}=2\theta_r.}
$$

$A$ is dimensionless and $B$ has units of kelvins. The first omitted level has three times the first excitation [energy](../../../../../../energy-split.md), explaining the exponent in the error term.

At high [temperature](../../../../../../temperature-split.md), $T\gg\theta_r$, many rotational levels are occupied and the sum can be replaced to leading order by an [integral](../../../../../../integral-split.md):

$$
Z_{\rm rot}\simeq\int_0^\infty(2J+1)e^{-(\theta_r/T)J(J+1)}\,dJ.
$$

Set $u=J(J+1)$, so that $du=(2J+1)dJ$. Then

$$
Z_{\rm rot}\simeq\int_0^\infty e^{-(\theta_r/T)u}\,du=\frac T{\theta_r}
=\frac{2Ik_B}{\hbar^2}T.
$$

Thus

$$
\boxed{C=\frac{2Ik_B}{\hbar^2}=\frac1{\theta_r},\qquad [C]=\mathrm{K^{-1}}.}
$$

The high-temperature approximation here concerns the rotational spectrum. For a real [molecule](../../../../../../molecule-split.md) it should still be used below [temperatures](../../../../../../temperature-split.md) where neglected vibrational excitation or dissociation invalidates the rigid-rotor model.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [C9](../../c9.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
