<h1 id="composite-simpson-s-rule">Composite Simpson's rule</h1>

↑ **Parent:** [Simpson's rule](simpson-s-rule.md)

[Composite Simpson's rule](composite-simpson-s-rule.md) applies [Simpson's rule](simpson-s-rule.md) to consecutive pairs of equal subintervals. Choose a positive even [integer](integer-split.md) $n\geq2$, put $h=(b-a)/n$, and take [quadrature nodes](quadrature-node.md) $x_j=a+jh$ for $j=0,\ldots,n$. There are $n$ subintervals, $n/2$ two-subinterval panels, and $n+1$ [quadrature nodes](quadrature-node.md). Then

$$
S_n=\frac h3\left[f(x_0)+4\sum_{j=1}^{n/2}f(x_{2j-1})+2\sum_{j=1}^{n/2-1}f(x_{2j})+f(x_n)\right].
$$

The second [sum](sum.md) is empty when $n=2$, recovering one panel. The [quadrature weights](quadrature-weight.md), before multiplication by $h/3$, are $1,4,2,4,\ldots,2,4,1$. Every interior even-indexed [quadrature node](quadrature-node.md) is an endpoint of two panels, so its two endpoint contributions add to two; every odd-indexed [quadrature node](quadrature-node.md) is a [midpoint](midpoint.md) with weight four. An odd $n$ cannot be covered by these pairs. The displayed formula requires equal spacing.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §5.6, equations 5.6.20–5.6.21: elementary and composite Simpson formulas](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/5-6-numerical-integration.md)

For the [exponential function](exponential-function.md) on the [interval](interval-mathematics.md) $[0,1]$, the exact [integral](integral-split.md) is $I=e-1$. With $n=2$, the formula gives $S_2\approx1.718861151876593$, an overestimate of about $5.793234175\times10^{-4}$. With $n=128$, it gives $S_{128}\approx1.718281828494607$, an overestimate of about $3.556140064\times10^{-11}$. The figure shows the intermediate refinements and compares every computed [absolute error](absolute-error.md) with the [error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md).

<a id="image-computed-composite-simpson-errors-for-the-exponential-function-on-zero-to-one-approach-fourth-order-convergence-the-dashed-curve-is-the-rigorous-bound-e-over-180-n-to-the-fourth-power"></a>
![](composite-simpson-exponential-convergence.png)

**[Figure 4](#image-computed-composite-simpson-errors-for-the-exponential-function-on-zero-to-one-approach-fourth-order-convergence-the-dashed-curve-is-the-rigorous-bound-e-over-180-n-to-the-fourth-power). Computed composite Simpson errors for the exponential function on zero to one approach fourth-order convergence; the dashed curve is the rigorous bound e over 180 n to the fourth power**.

For this [exponential function](exponential-function.md), a [geometric series](geometric-series.md) also gives a compact independent formula. With $q=e^h$ and $h=1/n$, summing the $n/2$ panel contributions yields

$$
S_n=(e-1)\frac{h(1+4q+q^2)}{3(q^2-1)}.
$$

A [Taylor series](taylor-series.md) at $h=0$ gives

$$
S_n-I=(e-1)\left(\frac{h^4}{180}-\frac{h^6}{1512}+O(h^8)\right).
$$

The [Big O notation](big-o-notation.md) describes the remaining terms as $h$ tends to zero. Consequently $(S_n-I)/(S_{2n}-I)$ tends to sixteen: the computed ratios increase from about $15.65169$ to $15.99965$. Fourth-order [truncation error](truncation-error.md) is also obtained by [Richardson extrapolation](richardson-extrapolation.md) of the [composite trapezoidal rule](composite-trapezoidal-rule.md).[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §5.6.2, equations 5.6.14–5.6.15: Simpson extrapolation and fourth-order error](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/5-6-numerical-integration.md)

**Table of contents**

- [Error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md)

## ↑ Ancestors (8)

1. [Simpson's rule](simpson-s-rule.md)
2. [Quadrature rule](quadrature-rule.md)
3. [Numerical integration](numerical-integration-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Composite Simpson's rule](composite-simpson-s-rule.md)
- [Error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md)
- [Simpson's rule](simpson-s-rule.md)
