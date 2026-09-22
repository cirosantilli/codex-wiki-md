# Composite midpoint quadrature rule

↑ **Parent:** [Midpoint quadrature rule](midpoint-quadrature-rule.md)

Apply the [midpoint quadrature rule](midpoint-quadrature-rule.md) on each of $n$ equal panels of a [partition of an interval](partition-of-an-interval.md), with $h=(b-a)/n$:

$$
M_n(f)=h\sum_{j=0}^{n-1}f\left(a+(j+\tfrac12)h\right).
$$

Each [quadrature node](quadrature-node.md) is a panel midpoint and each [quadrature weight](quadrature-weight.md) is $h$. For $f\in C^2[a,b]$, put $K=\max_{x\in[a,b]}|f''(x)|$. Summing the panel [quadrature errors](quadrature-error.md) gives

$$
M_n(f)-I(f)=-\frac{b-a}{24}h^2f''(\xi),\qquad |M_n(f)-I(f)|\leq\frac{b-a}{24}h^2K
$$

for some $\xi\in(a,b)$. Each panel contributes at most $Kh^3/24$; there are $n=(b-a)/h$ panels, explaining the [composite midpoint rule error](composite-midpoint-rule-error.md) of order $O(h^2)$ in [big O notation](big-o-notation.md). On a nonuniform [partition of an interval](partition-of-an-interval.md) with panel widths $h_j$ and largest width $H$, the corresponding bound is $K\sum_jh_j^3/24\leq K(b-a)H^2/24$.

For $f(x)=x^2$ on $[0,1]$, summing the sampled [polynomial](polynomial-split.md) exactly yields

$$
M_n(f)=\frac13-\frac{1}{12n^2}.
$$

Doubling $n$ divides the [absolute error](absolute-error.md) by exactly four. For a general $C^2$ [function](function-split.md), halving $h$ divides the displayed error bound by four, but the actual [absolute error](absolute-error.md) need not follow that ratio: cancellation can make it smaller or zero. [Continuous functions](continuous-function.md) still give convergence as the largest panel width tends to zero, by [uniform continuity](uniform-continuity.md); without the bounded second [derivative](derivative.md), the second-order rate is not guaranteed. [Noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md) explains a separate limitation when samples are inexact.

## ↑ Ancestors (6)

1. [Midpoint quadrature rule](midpoint-quadrature-rule.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Midpoint quadrature rule](midpoint-quadrature-rule.md)
- [Noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md)
- [Quadrature rule](quadrature-rule.md)
