<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $u=rF$. Multiplication of the radial equation by $-2mr/\hbar^2$ gives $u''+[A/r-\lambda(\lambda+1)/r^2-\alpha^2]u=0$. With $u=e^{-\alpha r}f$ the constant terms cancel, leaving

$$
\boxed{f''-2\alpha f'-\lambda(\lambda+1)f/r^2+Af/r=0.}
$$

The [indicial equation](../../../../indicial-equation.md) is $c(c-1)=\lambda(\lambda+1)$, with roots $c=\lambda+1$ and $c=-\lambda$. The usual physical [Coulomb radial origin condition](../../../../coulomb-radial-origin-condition.md) selects $c=\lambda+1$: it imposes the regular reduced radial boundary condition $u(0)=0$. Normalizability alone at the origin is insufficient to make this selection when an irregular branch is locally [square-integrable](../../../../square-integrable-function.md), notably at $\lambda=0$.

Write $f=r^{\lambda+1}\sum_{j\geq0}a_jr^j$. Coefficient comparison gives

$$
a_{j+1}=\frac{2\alpha(j+\lambda+1)-A}{(j+1)(j+2\lambda+2)}a_j.
$$

A nonterminating regular series has the exponentially growing asymptotic branch, suggested by $a_{j+1}/a_j\sim2\alpha/j$: it supplies an $e^{2\alpha r}$ component, which the prefactor $e^{-\alpha r}$ cannot normalize. Equivalently the regular confluent-hypergeometric solution grows unless its first parameter is a nonpositive integer. Thus a bound state requires the numerator to vanish at some $j=k\geq0$, giving

$$
\boxed{\alpha=\frac{A}{2(k+\lambda+1)},\qquad E=-\frac{\hbar^2A^2}{8m(k+\lambda+1)^2}.}
$$

This is [series-termination quantization of the Coulomb radial equation](../../../../series-termination-quantization-of-the-coulomb-radial-equation.md). It requires $A>0$ for the assumed $\alpha>0$; at $A=0$ there are no such negative-[energy](../../../../energy-split.md) Coulomb bound states.

For $k=0$, $F=Nr^\lambda e^{-\alpha r}$. The angular integral cancels when computing $\langle1/r\rangle$, while the radial volume element contributes $r^2dr$. Consequently

$$
\left\langle\frac1r\right\rangle=\frac{\int_0^\infty r^{2\lambda+1}e^{-2\alpha r}\,dr}{\int_0^\infty r^{2\lambda+2}e^{-2\alpha r}\,dr}=\frac{\alpha}{\lambda+1}.
$$

The ratio follows by one [integration by parts](../../../../integration-by-parts.md) and remains valid for real $\lambda\geq0$; no integer-only factorial identity is needed. Since now $\alpha=A/[2(\lambda+1)]$,

$$
\boxed{\langle V\rangle=-\frac{\hbar^2A\alpha}{2m(\lambda+1)}=-\frac{\hbar^2A^2}{4m(\lambda+1)^2}=2E.}
$$

For a classical particle with that negative total [energy](../../../../energy-split.md), nonnegative [kinetic energy](../../../../kinetic-energy.md) requires $E-V=\hbar^2(A/r-\alpha^2)/(2m)\geq0$, hence $\boxed{r\leq A/\alpha^2}$. This is a necessary radial bound; extra angular momentum can impose a stronger restriction.

At $k=\lambda=0$, $\alpha=A/2$ and the classical boundary is $r=2/\alpha$. The normalized radial [probability](../../../../probability.md) density is $4\alpha^3r^2e^{-2\alpha r}$. With $z=2\alpha r$, the exterior quantum [probability](../../../../probability.md) is

$$
\boxed{\int_{2/\alpha}^\infty4\alpha^3r^2e^{-2\alpha r}\,dr=\frac12\int_4^\infty z^2e^{-z}\,dz=13e^{-4}.}
$$

The final integration gives $(4^2+2\cdot4+2)e^{-4}/2$. This is the nonzero quantum tail beyond the classical turning region.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
