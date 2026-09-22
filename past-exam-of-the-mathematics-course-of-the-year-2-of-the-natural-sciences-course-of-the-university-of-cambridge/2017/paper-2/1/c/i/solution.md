<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $Y=\sum_{n\geq0}b_ny_n$ in the complete [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md). To determine $b_m$, multiply the differential equation by $y_m$ and integrate. The [Sturm-Liouville operator](../../../../../../sturm-liouville-operator.md) has the symmetry identity

$$
\int_0^1\big(y_m\mathcal LY-Y\mathcal Ly_m\big)\,dx=\big[p(Yy_m'-y_mY')\big]_0^1=0,
$$

because both functions obey the homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md). Consequently

$$
\lambda_m\int_0^1wYy_m\,dx=\alpha\int_0^1wYy_m\,dx+\int_0^1wfy_m\,dx,
$$

so that $(\lambda_m-\alpha)b_m=a_m$. The stipulated exclusion of every [eigenvalue](../../../../../../eigenvalue.md) makes all denominators nonzero, and gives

$$
\boxed{Y(x)=\sum_{n=0}^\infty\frac{a_n}{\lambda_n-\alpha}y_n(x).}
$$

This is the [resolvent operator](../../../../../../resolvent-of-an-operator.md) applied to $f$ in the weighted space. The same projection shows [uniqueness](../../../../../../uniqueness.md): a homogeneous solution would have $(\lambda_m-\alpha)b_m=0$ for every $m$, hence would vanish by completeness. For the regular problem the formula gives the solution in the operator domain when $f$ is square-integrable.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
