<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [monomial](../../../../monomial.md) $x^k$ lies in $\Pi_n$ and already fits the data. Uniqueness of [polynomial interpolation](../../../../polynomial-interpolation.md) therefore gives

$$
\boxed{p_n(x)=x^k.}
$$

Apply this result with a nonnegative integer $m\leq n$. Its [Lagrange interpolation](../../../../lagrange-polynomial.md) representation is the [polynomial identity](../../../../polynomial-identity.md)

$$
x^m=\sum_{i=0}^n x_i^m
\frac{\prod_{j\ne i}(x-x_j)}{\prod_{j\ne i}(x_i-x_j)}.
$$

The numerator in each summand is a [monic polynomial](../../../../monic-polynomial.md) of degree $n$, so the coefficient of $x^n$ on the right is exactly $\sum_i x_i^m/\prod_{j\ne i}(x_i-x_j)$. The coefficient on the left is zero for $m<n$ and one for $m=n$. Comparing coefficients proves the [Lagrange leading-coefficient identity](../../../../lagrange-leading-coefficient-identity.md)

$$
\boxed{\sum_{i=0}^n\frac{x_i^m}{\prod_{j\ne i}(x_i-x_j)}
=\begin{cases}0,&0\leq m<n,\\1,&m=n.\end{cases}}
$$

The intended exponent range is $m\geq0$: arbitrary negative exponents would not give this [polynomial identity](../../../../polynomial-identity.md). For $m=0$, $x_i^0$ denotes the value of the constant [polynomial](../../../../polynomial-split.md) $1$, including at a zero [interpolation node](../../../../interpolation-node.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
