<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

Assume the usual continuous-coefficient setting for a [second-order linear differential equation](../../../../../second-order-linear-differential-equation.md). The [Wronskian](../../../../../wronskian.md) $W=y_1y_2'-y_1'y_2$ has derivative

$$
W'=y_1y_2''-y_1''y_2=-p(x)W,
\qquad
W(x)=W(x_0)\exp\!\left[-\int_{x_0}^xp(s)\,ds\right],
$$

which proves the [Abel identity](../../../../../abel-s-identity.md). If $W(x_0)=0$, the two initial-value columns are [linearly dependent](../../../../../linear-dependence.md), so some nonzero $(\alpha,\beta)$ gives $\alpha y_1(x_0)+\beta y_2(x_0)=0$ and $\alpha y_1'(x_0)+\beta y_2'(x_0)=0$. The [uniqueness theorem for ordinary differential equations](../../../../../uniqueness-theorem-for-ordinary-differential-equations.md) makes that linear combination identically zero. If $W(x_0)\ne0$, the initial-value matrix is an [invertible matrix](../../../../../invertible-matrix.md), giving

$$
\boxed{a=\frac{Ay_2'(x_0)-By_2(x_0)}{W(x_0)},\qquad
b=\frac{By_1(x_0)-Ay_1'(x_0)}{W(x_0)}.}
$$

This establishes the alternative and supplies any prescribed initial data.

For the [Airy ordinary differential equation](../../../../../airy-ordinary-differential-equation.md), substitute a [power series](../../../../../power-series.md) $y=\sum_{m\geq0}a_mx^m$. Coefficient comparison gives $a_2=0$ and

$$
a_{m+3}=\frac{a_m}{(m+3)(m+2)},\qquad m\geq0.
$$

Choose $(a_0,a_1)=(1,0)$ and $(0,1)$. The [Airy power-series fundamental pair](../../../../../airy-power-series-fundamental-pair.md) is

$$
\boxed{y_1(x)=\sum_{k=0}^\infty
\frac{x^{3k}}{\prod_{j=1}^k(3j)(3j-1)},\qquad
y_2(x)=\sum_{k=0}^\infty
\frac{x^{3k+1}}{\prod_{j=1}^k(3j)(3j+1)}.}
$$

Empty products mean one. Their first terms are $y_1=1+x^3/6+x^6/180+\cdots$ and $y_2=x+x^4/12+x^7/504+\cdots$. The [ratio test](../../../../../ratio-test.md) gives convergence for every finite $x$, so termwise differentiation verifies the equation. Their [Wronskian](../../../../../wronskian.md) is one at zero, and hence everywhere because $p=0$. Thus every solution is $Ay_1+By_2$.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
