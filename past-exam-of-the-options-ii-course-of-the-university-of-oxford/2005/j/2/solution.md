<h1 id="j/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Set](../../../../set-split.md) $u=r\psi$, choose $\alpha>0$ for a negative bound-state energy, and write $\kappa=2mK/\hbar^2$. Multiplying the radial equation by $r$ gives

$$
u''+\left[-\alpha^2+\frac\kappa r-\frac{\ell(\ell+1)}{r^2}\right]u=0.
$$

For $u=e^{-\alpha r}f$, its [second derivative](../../../../second-derivative.md) is $e^{-\alpha r}(f''-2\alpha f'+\alpha^2f)$. Substitution cancels the two $\alpha^2$ terms and gives

$$
\boxed{f''-2\alpha f'-\frac{\ell(\ell+1)}{r^2}f+\frac\kappa r f=0.}
$$

For the physical hydrogen problem, the angular eigenvalue has $\ell$ a [nonnegative integer](../../../../natural-number.md). Regularity at the origin selects the Frobenius exponent $u\sim r^{\ell+1}$, rather than the singular branch. Put

$$
f=r^{\ell+1}\sum_{j=0}^\infty c_jr^j.
$$

The equation for the [series](../../../../series-mathematics.md) factor $v=f/r^{\ell+1}$ is $rv''+(2\ell+2-2\alpha r)v'+(\kappa-2\alpha(\ell+1))v=0$, and coefficient comparison yields

$$
c_{j+1}=\frac{2\alpha(j+\ell+1)-\kappa}{(j+1)(j+2\ell+2)}c_j.
$$

The regular confluent-hypergeometric solution generically grows like $e^{2\alpha r}$ in this [series](../../../../series-mathematics.md) factor; after the extracted $e^{-\alpha r}$ it is not [normalizable](../../../../normalizable-wavefunction.md). A [bound state](../../../../bound-state.md) requires termination at some degree $q\ge0$, namely $2\alpha(q+\ell+1)=\kappa$. Thus $n=q+\ell+1$ is an [integer](../../../../integer-split.md) greater than $\ell$, and

$$
\boxed{\alpha=\frac{mK}{\hbar^2n},\qquad E_n=-\frac{mK^2}{2\hbar^2n^2}.}
$$

Regularity, normalizability and the [integer](../../../../integer-split.md) angular index are the physical conditions selecting this spectrum; the [differential equation](../../../../differential-equation-split.md) without those conditions would admit many other solutions.

For $n=1$, necessarily $\ell=0$ and $q=0$. With $a_0=\hbar^2/(mK)$,

$$
\boxed{f_1(r)=Cr,\qquad\psi_1(r)=Ce^{-r/a_0}.}
$$

A normalized spatial [ground state](../../../../ground-state.md) is $\Psi_1=(\pi a_0^3)^{-1/2}e^{-r/a_0}$. In [spherical coordinates](../../../../spherical-coordinate-system.md) the radial [probability](../../../../probability.md) has weight $r^2dr$. Constants and the angular [integral](../../../../integral-split.md) cancel in the tail ratio. The supplied [integral](../../../../integral-split.md) with $\lambda=2/a_0$ gives

$$
\Pr(r>a_0)=\frac{\int_{a_0}^\infty r^2e^{-2r/a_0}\,dr}{\int_0^\infty r^2e^{-2r/a_0}\,dr}
=e^{-2}(1+2+2)=\boxed{5e^{-2}}.
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [J](../../j.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
