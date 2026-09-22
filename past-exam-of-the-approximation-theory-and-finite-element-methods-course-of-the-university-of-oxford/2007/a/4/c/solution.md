<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\beta(q)$ be the centered nondimensional cubic [B-spline](../../../../../b-spline.md), even and supported on $[-2,2]$. The outer cubic must be $b(2-|q|)^3$ to make the function and its first two [derivatives](../../../../../derivative.md) vanish at the support edge. Write its inner part as $A+Bq^2+C|q|^3$. Matching the value and first two [derivatives](../../../../../derivative.md) at $|q|=1$ gives $A=4b$, $B=-6b$, $C=3b$. Its nonzero knot values are then $4b,b,b$, so requiring their sum to be one fixes $b=1/6$. Thus

$$
\boxed{\beta(q)=
\begin{cases}
(4-6q^2+3|q|^3)/6,&|q|\leq1,\\
(2-|q|)^3/6,&1\leq|q|\leq2,\\
0,&|q|\geq2.
\end{cases}}
$$

In particular $\beta(0)=2/3$, $\beta(\pm1)=1/6$.

With $h=1/m$, represent the [spline](../../../../../spline-mathematics.md) on $[0,1]$ as $s(x)=\sum_{j=-1}^{m+1}c_j\beta(x/h-j)$. There are $m+3$ unknown coefficients. [interpolation](../../../../../interpolation-split.md) at $x_i=ih$, $0\leq i\leq m$, gives

$$
c_{i-1}+4c_i+c_{i+1}=6\sqrt{1-ih}.
$$

The natural endpoint conditions, using $\beta''(0)=-2$ and $\beta''(\pm1)=1$, give

$$
c_{-1}-2c_0+c_1=0,\qquad
c_{m-1}-2c_m+c_{m+1}=0.
$$

These $m+3$ equations are the required [matrix](../../../../../matrix.md) system: the $m+1$ [interpolation](../../../../../interpolation-split.md) rows have coefficients $(1,4,1)$ at consecutive positions and right sides $6u(x_i)$; the two endpoint rows have $(1,-2,1)$ and zero right sides. No solution of that system is required. The scaling uses $\beta(x/h-j)$, without an extra $1/h$, because normalization is by knot values rather than by integral.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
