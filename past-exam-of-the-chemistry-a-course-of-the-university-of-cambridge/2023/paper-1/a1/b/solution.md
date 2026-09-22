<h1 id="a1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep one normalized [spin](../../../../../spin.md) function fixed and write $A=1/\sqrt{24}$ and $f_m(\theta,\phi)=\sin\theta\,e^{im\phi}$, with $m=\pm1$. Overall constants and the [spin](../../../../../spin.md) factor pass unchanged through the spatial operators.

First, in [atomic units](../../../../../atomic-units.md), $\hat l_z=-i\partial_\phi$, so

$$
\hat l_z\Psi=-i(im)\Psi=\boxed{m\Psi}.
$$

For the squared [orbital angular momentum](../../../../../orbital-angular-momentum.md), $\partial_\phi^2f_m=-f_m$ and

$$
\partial_\theta\!\left(\sin\theta\,\partial_\theta f_m\right)
=(\cos^2\theta-\sin^2\theta)e^{im\phi}.
$$

Therefore the two terms of the angular operator give

$$
\hat l^2f_m=
\frac{-\cos^2\theta+\sin^2\theta+1}{\sin\theta}e^{im\phi}
=2\sin\theta e^{im\phi}=2f_m,
$$

using $1-\cos^2\theta=\sin^2\theta$. Thus **$\hat l^2\Psi=2\Psi$**.

Finally, the spatial hydrogen [Hamiltonian](../../../../../hamiltonian.md) is

$$
\hat H=-\frac12\left[\frac{1}{r^2}\partial_r(r^2\partial_r)-\frac{\hat l^2}{r^2}\right]-\frac1r.
$$

For $R=Ar e^{-r/2}$,

$$
R'=A(1-r/2)e^{-r/2},\qquad
\frac1{r^2}\frac{\mathrm d}{\mathrm dr}(r^2R')
=Ae^{-r/2}\left(\frac2r-2+\frac r4\right).
$$

Substitute the already established angular [eigenvalue](../../../../../eigenvalue.md) $l(l+1)=2$:

$$
\hat H(RY\sigma)=AY\sigma e^{-r/2}
\left[-\frac12\left(\frac2r-2+\frac r4\right)+\frac1r-1\right]
=-\frac18RY\sigma.
$$

Hence **$E=-1/8$ hartree**, consistently with $n=2$. The angular calculation must precede the radial substitution if one wants to avoid differentiating the entire product repeatedly.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [A1](../../a1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
