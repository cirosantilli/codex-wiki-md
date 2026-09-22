<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are $n+2$ distinct [interpolation nodes](../../../../interpolation-node.md) but only $n+1$ free [coefficients](../../../../coefficient.md) in a [polynomial](../../../../polynomial-split.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n$. Thus [polynomial interpolation](../../../../polynomial-interpolation.md) is possible precisely when the data satisfy one compatibility equation. To identify it, form the [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md) through all the data:

$$
q(x)=\sum_{i=0}^{n+1}f_i
\prod_{\substack{0\leq j\leq n+1\\j\ne i}}
\frac{x-x_j}{x_i-x_j}.
$$

This is the unique [interpolation polynomial](../../../../interpolation-polynomial.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n+1$. Its [leading coefficient](../../../../leading-coefficient-of-a-polynomial.md), which is also the order-$(n+1)$ [divided difference](../../../../divided-difference.md), is

$$
D=\sum_{i=0}^{n+1}\frac{f_i}
{\displaystyle\prod_{\substack{0\leq j\leq n+1\\j\ne i}}(x_i-x_j)}.
$$

Consequently the required condition is

$$
\boxed{D=0.}
$$

Necessity follows because any qualifying $p_n$ must equal $q$ by uniqueness of [polynomial interpolation](../../../../polynomial-interpolation.md); sufficiency follows because $D=0$ removes the only possible term of [polynomial degree](../../../../degree-of-a-polynomial.md) $n+1$ from $q$.

When this condition holds, a slightly shorter expression uses only the first $n+1$ [interpolation nodes](../../../../interpolation-node.md):

$$
\boxed{p_n(x)=\sum_{i=0}^{n}f_i
\prod_{\substack{0\leq j\leq n\\j\ne i}}
\frac{x-x_j}{x_i-x_j}.}
$$

This [polynomial](../../../../polynomial-split.md) agrees with $q$ at $n+1$ distinct points, so the [root bound for a polynomial](../../../../lagrange-root-bound-over-a-field.md) gives $p_n=q$ and hence $p_n(x_{n+1})=f_{n+1}$ as required. Equivalently, the compatibility condition says that this expression, evaluated at the last [interpolation node](../../../../interpolation-node.md), gives $f_{n+1}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
