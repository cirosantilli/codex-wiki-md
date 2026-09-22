<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Multiply the linear [stochastic differential equation](../../../../../../stochastic-differential-equation.md) by $e^{-at}$. The [Itô product rule](../../../../../../ito-product-rule.md) gives

$$
Z_t=e^{at}z+b\int_0^t e^{a(t-s)}\,dW_s.
$$

The integrand is deterministic, so the [Itô integral](../../../../../../ito-integral.md) has a centered [normal distribution](../../../../../../normal-distribution.md). Its [variance](../../../../../../variance-split.md), by the [Itô isometry](../../../../../../ito-isometry.md), is

$$
b^2\int_0^t e^{2a(t-s)}ds
=\begin{cases}\displaystyle\frac{b^2}{2a}(e^{2at}-1),&a\ne0,\\b^2t,&a=0.\end{cases}
$$

Hence

$$
\boxed{Z_t\sim N\left(e^{at}z,\frac{b^2}{2a}(e^{2at}-1)\right)\quad(a\ne0).}
$$

At $a=0$ the correct continuous-limit formula is $N(z,b^2t)$. A zero [variance](../../../../../../variance-split.md), for example when $b=0$, denotes the deterministic distribution. For $a<0$ the [variance](../../../../../../variance-split.md) is still positive because both numerator and denominator in its quotient are negative. This is the [explicit Ornstein-Uhlenbeck solution](../../../../../../explicit-ornstein-uhlenbeck-solution.md), allowing either sign of the linear drift coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
