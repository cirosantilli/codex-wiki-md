<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Separate the interior [Helmholtz equation](../../../../../helmholtz-equation.md) in the same angular basis. Each radial coefficient $F_\ell(r)$ satisfies

$$
\boxed{r^2F_\ell''+2rF_\ell'+[sr^2-\ell(\ell+1)]F_\ell=0.}
$$

For $s>0$, set $x=\sqrt{s}\,r$. The equation becomes $x^2f_\ell''+2xf_\ell'+[x^2-\ell(\ell+1)]f_\ell=0$. Its regular solution is a [Spherical Bessel function](../../../../../spherical-bessel-function.md) $j_\ell(x)$, up to a multiplicative constant. The second independent solution is singular as $r^{-\ell-1}$ at the origin and is excluded. Hence

$$
\boxed{B_{\rm in}(r,\theta)=\sum_{\ell=0}^\infty B_\ell j_\ell(\sqrt{s}\,r)P_\ell(\cos\theta).}
$$

One may denote $j_\ell$ by $f_\ell$ as in the source. Its leading behaviour $j_\ell(x)\sim x^\ell/(2\ell+1)!!$ ensures regularity. Primes on $j_\ell$ below refer to its dimensionless argument; differentiating with respect to $r$ introduces the factor $\sqrt{s}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
