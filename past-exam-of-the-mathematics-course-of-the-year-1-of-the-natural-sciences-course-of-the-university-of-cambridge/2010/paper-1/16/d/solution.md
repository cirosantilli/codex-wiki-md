<h1 id="16/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Multiply the two defining [Gamma integrals](../../../../../gamma-integral.md). For $p,q>0$ the nonnegative product integrand allows [Tonelli's theorem](../../../../../tonelli-theorem.md):

$$
\Gamma(p)\Gamma(q)=\int_0^\infty\int_0^\infty x^{p-1}y^{q-1}e^{-(x+y)}dx\,dy.
$$

Use $r=x+y$, $u=x/(x+y)$, so $x=ru$, $y=r(1-u)$ and the positive quadrant becomes $r>0$, $0<u<1$. The [Jacobian determinant](../../../../../jacobian-determinant.md) has absolute value

$$
\left|\det\begin{pmatrix}u&r\\1-u&-r\end{pmatrix}\right|=r.
$$

After including this factor, the transformed integral separates:

$$
\left[\int_0^\infty r^{p+q-1}e^{-r}dr\right]
\left[\int_0^1u^{p-1}(1-u)^{q-1}du\right]
=\Gamma(p+q)B(p,q).
$$

This proves the [beta-gamma identity](../../../../../beta-gamma-identity.md),

$$
\boxed{\Gamma(p)\Gamma(q)=B(p,q)\Gamma(p+q).}
$$

All changes of variables are made inside the open positive domains; their boundaries do not contribute to the integrals.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
