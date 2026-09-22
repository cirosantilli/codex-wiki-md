<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

Differentiate the [Legendre differential equation](../../../../../legendre-differential-equation.md) once and put $R_n=P_n'$:

$$
(1-x^2)R_n''-4xR_n'+\bigl(n(n+1)-2\bigr)R_n=0.
$$

Multiplying by $1-x^2$ gives its [Sturm-Liouville form](../../../../../sturm-liouville-form.md),

$$
\boxed{-\frac{d}{dx}\left[(1-x^2)^2R_n'\right]
=\lambda_n(1-x^2)R_n,\qquad \lambda_n=(n-1)(n+2).}
$$

Thus the weight is $w(x)=1-x^2$, not one. For $n\ge1$, $R_n$ is a nonzero polynomial; $R_0=0$ is a trivial solution rather than a nonzero [eigenfunction](../../../../../eigenfunction.md).

Multiply the equations for $n,m$ by $R_m,R_n$ respectively, subtract and integrate. The resulting boundary term is $[(1-x^2)^2(R_n'R_m-R_m'R_n)]_{-1}^1=0$, since all these derivatives are finite at the endpoints. For distinct nonnegative indices, $\lambda_n-\lambda_m\ne0$, giving the [weighted orthogonality of Legendre polynomial derivatives](../../../../../weighted-orthogonality-of-legendre-polynomial-derivatives.md):

$$
\boxed{\int_{-1}^1(1-x^2)R_n(x)R_m(x)\,dx=0\quad(n\ne m).}
$$

For $n=0$ the integral is zero simply because $R_0=0$.

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
