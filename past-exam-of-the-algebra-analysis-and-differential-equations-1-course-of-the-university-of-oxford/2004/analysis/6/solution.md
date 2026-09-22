<h1 id="analysis/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

After division by $z(z+2)$, the coefficients are

$$
p(z)=\frac{z+1}{z(z+2)},\qquad q(z)=-\frac{\alpha^2}{z(z+2)}.
$$

Their only finite singularities are **$z=0$ and $z=-2$**. At either point $z_0$, the products $(z-z_0)p$ and $(z-z_0)^2q$ are analytic, so both points are regular singular points. All other finite points are ordinary.

The lowest power after substituting the [Frobenius series](../../../../frobenius-solution.md) gives $\sigma(2\sigma-1)=0$. The coefficient of $z^{n+\sigma}$ then gives

$$
\boxed{\sigma=0\text{ or }\frac12,\qquad a_{n+1}=\frac{\alpha^2-(n+\sigma)^2}{(n+\sigma+1)(2n+2\sigma+1)}a_n.}
$$

For both exponents the denominator is nonzero for every $n\geq0$, so each arbitrary nonzero $a_0$ determines a series. Unless it terminates, its coefficient ratio tends to $-1/2$, proving convergence for $|z|<2$. For the half-integer exponent choose a square-root branch. Their leading powers $1$ and $z^{1/2}$ show that the two local solutions are [linearly independent](../../../../linear-independence.md).

If $\alpha=m$ is a [positive integer](../../../../positive-integer.md), choose $\sigma=0$. The recurrence numerator is nonzero for $0\leq n<m$ and vanishes at $n=m$. Thus $a_m\ne0$, $a_{m+1}=0$, and all later coefficients vanish: **a [polynomial](../../../../polynomial-split.md) solution of exact degree $m$ exists**. It is proportional to the [Chebyshev polynomial](../../../../chebyshev-polynomial.md) $T_m(z+1)$, since the substitution $t=z+1$ transforms the equation into $(t^2-1)y''+ty'-m^2y=0$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Analysis](../../analysis.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
