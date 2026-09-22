<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For the two inline operator labels, **(a)** $L_z$ has [eigenvalue](../../../../../eigenvalue.md) $m_\ell\hbar$, and **(b)** $L^2$ has [eigenvalue](../../../../../eigenvalue.md) $\ell(\ell+1)\hbar^2$, with $\ell=0,1,\ldots$ and $m_\ell=-\ell,\ldots,\ell$. The subscript distinguishes the [magnetic quantum number](../../../../../magnetic-quantum-number.md) from the [electron](../../../../../electron.md) [mass](../../../../../mass.md).

Put $b=a_0(\ell+1)$ and $\kappa=e^2/(4\pi\epsilon_0)$. For the proposed radial shape,

$$
\frac1{r^2R}\frac{d}{dr}\left(r^2\frac{dR}{dr}\right)
=\frac{\ell(\ell+1)}{r^2}-\frac{2(\ell+1)}{br}+\frac1{b^2}.
$$

The angular-momentum term cancels the inverse-square part. The inverse-radius coefficient vanishes if $\hbar^2(\ell+1)/(mb)=\kappa$. Therefore

$$
\boxed{a_0=\frac{4\pi\epsilon_0\hbar^2}{me^2}},\qquad
\boxed{E=-\frac{\hbar^2}{2ma_0^2(\ell+1)^2}}.
$$

This [nodeless Coulomb radial eigenstate](../../../../../nodeless-coulomb-radial-eigenstate.md) has [principal quantum number](../../../../../principal-quantum-number.md) $n=\ell+1$, not the complete set of hydrogen radial states. Since the [spherical harmonic](../../../../../spherical-harmonic.md) is normalized, radial normalization requires

$$
1=|A|^2(2\ell+2)!\left(\frac b2\right)^{2\ell+3},\qquad
\boxed{A=\frac{(2/b)^{\ell+3/2}}{\sqrt{(2\ell+2)!}}}
$$

up to an arbitrary [phase](../../../../../phase-waves.md).

For the [hydrogen ground-state nuclear-volume probability](../../../../../hydrogen-ground-state-nuclear-volume-probability.md), use $R=2a_0^{-3/2}e^{-r/a_0}$. With $u=r_p/a_0\ll1$,

$$
P(r<r_p)=1-e^{-2u}(1+2u+2u^2)
\simeq\boxed{\frac43\left(\frac{r_p}{a_0}\right)^3}.
$$

No numerical [proton](../../../../../proton.md) radius is supplied or required. A sharp [proton](../../../../../proton.md) boundary is an approximation to a charge distribution, and the point-Coulomb potential changes inside an extended [proton](../../../../../proton.md). Finite [proton](../../../../../proton.md) [mass](../../../../../mass.md), relativistic and electromagnetic corrections also limit the ideal [wavefunction](../../../../../wave-function-split.md)'s precision.

Classically the [kinetic energy](../../../../../kinetic-energy.md) must satisfy $E-V(r)\geq0$. For $E=-\kappa/(2a_0)$ this demands **$r\leq2a_0$**. The [hydrogen ground-state probability beyond the classical turning point](../../../../../hydrogen-ground-state-probability-beyond-the-classical-turning-point.md) is

$$
P(r>2a_0)=\int_{2a_0}^\infty\frac{4r^2}{a_0^3}e^{-2r/a_0}\,dr
=\boxed{13e^{-4}\simeq0.238}.
$$

A substantial [probability](../../../../../probability.md) lies beyond the classical turning radius; the bound-state [wavefunction](../../../../../wave-function-split.md) decays there rather than vanishing.

<a id="section-b/b9/image-original-hydrogen-ground-state-radial-probability-density-with-its-classically-forbidden-tail-shaded"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1-hydrogen-tail.png)

**[Figure 2](#section-b/b9/image-original-hydrogen-ground-state-radial-probability-density-with-its-classically-forbidden-tail-shaded). Original hydrogen ground-state radial probability density with its classically forbidden tail shaded**.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
