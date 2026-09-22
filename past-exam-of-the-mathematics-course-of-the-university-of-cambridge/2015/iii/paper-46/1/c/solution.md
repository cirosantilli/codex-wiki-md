<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After integrating out the shell, let a chosen operator's coefficient be $\kappa+\Delta\kappa$ and write the two-derivative quadratic term as $\tfrac12(1+\Delta Z)(\partial\phi)^2$. Here $\Delta\kappa$ is the shell-induced change before rescaling, and $\Delta Z$ is the shell correction to the [wavefunction renormalization](../../../../../../wave-function-renormalization.md). Work in an operator basis in which that quadratic term has this form; the other generated operators remain in the [Wilsonian effective action](../../../../../../wilsonian-effective-action.md).

Under $x'=bx$, the volume element changes by $d^4x=b^{-4}d^4x'$ and each derivative by $\partial_x=b\partial_{x'}$. [Canonical field normalization](../../../../../../canonical-field-normalization.md) is restored by defining

$$
\phi'(x')=b^{-1}\sqrt{1+\Delta Z}\,\phi(x'/b),\qquad
\phi(x)=\frac b{\sqrt{1+\Delta Z}}\phi'(bx).
$$

Indeed, the volume factor, two derivatives and two field factors cancel in the [kinetic term](../../../../../../kinetic-term.md). A term with $n$ fields and $m$ derivatives consequently obtains the factor $b^{-4}b^m b^n(1+\Delta Z)^{-n/2}$. Hence

$$
\boxed{\kappa'=\frac{\kappa+\Delta\kappa}{(1+\Delta Z)^{n/2}}\,b^{m+n-4}
=\frac{\kappa+\Delta\kappa}{(1+\Delta Z)^{n/2}}\left(\frac{\Lambda'}\Lambda\right)^{m+n-4}.}
$$

This is [Wilsonian rescaling of a scalar coupling](../../../../../../wilsonian-rescaling-of-a-scalar-coupling.md). The exponent is minus the coupling's engineering [mass dimension](../../../../../../mass-dimension.md), $[\kappa]=4-n-m$. The rescaling also returns the low-momentum cutoff to $\Lambda$, because $p'=p/b$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
