<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On a [partition of an interval](../../../../../partition-of-an-interval.md) $a=x_0<x_1<\cdots<x_N=b$, apply the [trapezoidal rule](../../../../../trapezoidal-rule.md) separately to each panel and add:

$$
\boxed{T_N(f)=\sum_{j=1}^N\frac{x_j-x_{j-1}}2\bigl(f(x_{j-1})+f(x_j)\bigr).}
$$

For uniform spacing $h=(b-a)/N$, this [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md) becomes

$$
\boxed{T_N(f)=h\left[\frac12f(a)+\sum_{j=1}^{N-1}f(a+jh)+\frac12f(b)\right].}
$$

Each interior sample occurs in two panels; their half-[quadrature weights](../../../../../quadrature-weight.md) combine to $h$. The endpoint [quadrature weights](../../../../../quadrature-weight.md) are $h/2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
