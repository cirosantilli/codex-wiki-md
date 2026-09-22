<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h=(b-a)/n$, $x_j=a+jh$, and $m_j=a+(j+\tfrac12)h$. The [composite midpoint rule](../../../../../composite-midpoint-quadrature-rule.md) and [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md) are

$$
M_n=h\sum_{j=0}^{n-1}f(m_j),\qquad
T_n=h\left[\frac{f(a)+f(b)}2+\sum_{j=1}^{n-1}f(x_j)\right].
$$

For [composite Simpson's rule](../../../../../composite-simpson-s-rule.md) with $2n$ strips, the spacing is $h/2$. Its odd-indexed nodes are the $m_j$ and its even interior nodes are the $x_j$. Consequently

$$
\begin{aligned}
S_{2n}
&=\frac h6\left[f(a)+f(b)+4\sum_{j=0}^{n-1}f(m_j)+2\sum_{j=1}^{n-1}f(x_j)\right]\\
&=\boxed{\frac23M_n+\frac13T_n}.
\end{aligned}
$$

This is an identity between the [quadrature rules](../../../../../quadrature-rule.md), not an approximation involving an omitted [quadrature error](../../../../../quadrature-error.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
