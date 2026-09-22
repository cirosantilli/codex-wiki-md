<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

Differentiate the [Legendre differential equation](../../../../../legendre-differential-equation.md) and put $Q_n=P_n'$. This gives

$$
(1-x^2)Q_n''-4xQ_n'+(n-1)(n+2)Q_n=0.
$$

Multiplication by $1-x^2$ puts it in the [self-adjoint form](../../../../../sturm-liouville-theory.md)

$$
\boxed{
\frac d{dx}\left((1-x^2)^2Q_n'\right)
 +(n-1)(n+2)(1-x^2)Q_n=0}.
$$

The boundary term vanishes at $x=\pm1$. Distinct eigenvalues are therefore orthogonal with weight $1-x^2$:

$$
\boxed{
\int_{-1}^{1}(1-x^2)Q_n(x)Q_m(x),dx=0,
\qquad n\ne m.}
$$

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
