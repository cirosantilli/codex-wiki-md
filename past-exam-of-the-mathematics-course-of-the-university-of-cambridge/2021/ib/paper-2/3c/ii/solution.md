<h1 id="3c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $y=e^{-x}u$. Then

$$
y''+2y'=e^{-x}(u''-u),
$$

so the eigenvalue equation becomes

$$
u''+(\lambda-1)u=0,
\qquad u(0)=u(1)=0.
$$

The [Dirichlet eigenvalues](../../../../../../dirichlet-eigenvalue.md) and corresponding eigenfunctions are therefore

$$
\boxed{\lambda_n=1+n^2\pi^2,\qquad
y_n(x)=e^{-x}\sin(n\pi x),\quad n\geq1}.
$$

They form an infinite discrete increasing set. Their weighted inner products satisfy

$$
\int_0^1w\,y_ny_m\,dx
=\int_0^1\sin(n\pi x)\sin(m\pi x)\,dx
=\frac12\delta_{nm}.
$$

Thus the [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md) coefficient is

$$
\boxed{
A_n=
\frac{\int_0^1e^{2x}(x-x^2)y_n(x)\,dx}
{\int_0^1e^{2x}y_n(x)^2\,dx}
=2\int_0^1e^x(x-x^2)\sin(n\pi x)\,dx }.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3C](../../3c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
