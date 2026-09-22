<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Define the [weighted inner product](../../../../weighted-inner-product.md) $\langle u,v\rangle_w=\int_a^bw(x)\overline{u(x)}v(x)dx$. For the stated operator $L=-(pD)' -q$, integration by parts gives the [Lagrange identity for a Sturm-Liouville operator](../../../../lagrange-identity-for-a-sturm-liouville-operator.md)

$$
\int_a^b[\overline uLv-\overline{Lu}v]dx=[p(\overline{u'}v-\overline u v')]_a^b.
$$

The endpoint terms vanish for [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md). Taking $u=v$ proves each eigenvalue is real, since $w>0$ makes the squared weighted norm positive. For eigenfunctions $u_m,u_n$ of distinct eigenvalues, the same identity gives $(\lambda_n-\lambda_m)\langle u_m,u_n\rangle_w=0$, proving their orthogonality.

For the specific equation, divide by $x^2$ to obtain $-y''=\lambda x^{-2}y$, so its weight is $w=x^{-2}$, with $p=1,q=0$. Put $v=\ln x$, $\ell=\ln2$ and $Y(v)=y(e^v)$. The [logarithmic change of variable in a Sturm-Liouville problem](../../../../logarithmic-change-of-variable-in-a-sturm-liouville-problem.md) gives $x^2y''=Y''-Y'$. Remove the first derivative with $Y=e^{v/2}Z$; the equation becomes $Z''+(\lambda-1/4)Z=0$, with $Z(0)=Z(\ell)=0$.

The [Dirichlet spectrum with inverse-square weight](../../../../dirichlet-spectrum-with-inverse-square-weight.md) is therefore

$$
\boxed{\lambda_n=\frac14+\left(\frac{n\pi}{\ln2}\right)^2,\qquad y_n(x)=\sqrt{\frac2{\ln2}}\sqrt x\sin\frac{n\pi\ln x}{\ln2},\quad n\geq1.}
$$

Indeed $\int_1^2x^{-2}y_my_n dx=(2/\ell)\int_0^\ell\sin(m\pi v/\ell)\sin(n\pi v/\ell)dv=\delta_{mn}$. Values $\lambda\leq1/4$ give a linear or hyperbolic transformed solution and no nonzero solution vanishing at both ends.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
