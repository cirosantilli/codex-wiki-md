<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

The origin is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md), since the coefficients of the [second-order linear differential equation](../../../../../second-order-linear-differential-equation.md) are [polynomials](../../../../../polynomial-split.md). Seek a [power series](../../../../../power-series.md) $y=\sum_{n\geq0}a_nx^n$. Matching the coefficients of $x^0$ and $x^1$ gives $a_2=a_3=0$. Matching the coefficient of $x^{j+2}$ gives

$$
(j+4)(j+3)a_{j+4}+(4j+1)a_j=0,
\qquad
\boxed{a_{j+4}=-\frac{4j+1}{(j+4)(j+3)}a_j\quad(j\geq0).}
$$

Thus the four residue classes of indices modulo four evolve separately. The [initial conditions](../../../../../initial-condition.md) for the first solution give $a_0=1$, $a_1=0$, and hence

$$
y_1(x)=\sum_{m=0}^{\infty}(-1)^m
\left(\prod_{j=0}^{m-1}\frac{16j+1}{(4j+4)(4j+3)}\right)x^{4m}
=1-\frac{x^4}{12}+\frac{17x^8}{672}-\frac{17x^{12}}{2688}+\cdots.
$$

The second set of [initial conditions](../../../../../initial-condition.md) gives $a_0=0$, $a_1=1$, and

$$
y_2(x)=\sum_{m=0}^{\infty}(-1)^m
\left(\prod_{j=0}^{m-1}\frac{16j+5}{(4j+5)(4j+4)}\right)x^{4m+1}
=x-\frac{x^5}{4}+\frac{7x^9}{96}-\frac{259x^{13}}{14976}+\cdots.
$$

An empty product equals one. In either [power series](../../../../../power-series.md), the ratio of successive nonzero terms tends to zero for every fixed $x$: the coefficient ratio is of order $1/m$, while the power increases by four. The [ratio test](../../../../../ratio-test.md) therefore proves convergence for every $x$, and termwise differentiation verifies the [differential equation](../../../../../differential-equation-split.md). These normalized solutions are [linearly independent](../../../../../linear-independence.md).

For their [Wronskian](../../../../../wronskian.md) $W=y_1y_2'-y_1'y_2$, differentiating and substituting the [differential equation](../../../../../differential-equation-split.md) gives

$$
W'=y_1y_2''-y_1''y_2=-4x^3W,\qquad W(0)=1.
$$

Thus the [Abel identity](../../../../../abel-s-identity.md) yields

$$
\boxed{W(x)=e^{-x^4}.}
$$

On the interval containing zero where $y_1$ has no zero,

$$
\left(\frac{y_2}{y_1}\right)'=\frac{W}{y_1^2}=\frac{e^{-x^4}}{y_1(x)^2}.
$$

Since $y_2(0)/y_1(0)=0$, integration proves the requested [reduction of order](../../../../../reduction-of-order.md) formula:

$$
\boxed{y_2(x)=y_1(x)\int_0^x\frac{e^{-\xi^4}}{y_1(\xi)^2}\,d\xi.}
$$

This is a local formula around the origin, as requested. The [power series](../../../../../power-series.md) define both solutions globally; an ordinary integral through a zero of $y_1$ is not intended. [Reduction of order across a zero of the known solution](../../../../../reduction-of-order-across-a-zero-of-the-known-solution.md) instead uses continuation of the actual solution.

## ↑ Ancestors (11)

1. [5B](../5b.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
