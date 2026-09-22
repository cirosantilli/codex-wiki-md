<h1 id="error-bound-for-composite-simpson-s-rule">Error bound for composite Simpson's rule</h1>

↑ **Parent:** [Composite Simpson's rule](composite-simpson-s-rule.md)

Suppose $f$ has a fourth [derivative](derivative.md) that is a [continuous function](continuous-function.md) on the [interval](interval-mathematics.md) $[a,b]$, and $|f^{(4)}(x)|\leq M$ there. With $I=\int_a^b f(x)\,dx$, the signed [quadrature error](quadrature-error.md) here is $I-S_n$. Then, for some [point](point-geometry.md) $\xi\in(a,b)$,

$$
I-S_n=-\frac{b-a}{180}h^4 f^{(4)}(\xi),\qquad
|I-S_n|\leq\frac{M(b-a)}{180}h^4.
$$

In particular, a strictly positive fourth [derivative](derivative.md) makes $I-S_n<0$: [composite Simpson's rule](composite-simpson-s-rule.md) overestimates the [integral](integral-split.md).[NIST Digital Library of Mathematical Functions; §3.5(ii), equations 3.5.6–3.5.8: continuous fourth derivative, elementary remainder, composite formula and signed error](nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-ii-simpson%E2%80%99s-rule.md)

The bound's scale follows by adding the panel errors. A panel of width $2h$ has signed [quadrature error](quadrature-error.md) $-h^5 f^{(4)}(\xi_j)/90$ and [absolute error](absolute-error.md) at most $Mh^5/90$. There are $(b-a)/(2h)$ panels, so the [triangle inequality](triangle-inequality.md) gives $M(b-a)h^4/180$. The [intermediate value theorem](intermediate-value-theorem.md) for the continuous fourth [derivative](derivative.md) replaces the average of the panel values $f^{(4)}(\xi_j)$ by a single value $f^{(4)}(\xi)$, giving the signed formula.

The underlying single-panel calculation can be seen through the [Peano kernel theorem](peano-kernel-theorem.md). On the [interval](interval-mathematics.md) $[0,2]$, define the raw [Peano kernel](peano-kernel.md) $K(t)=L[(x-t)_+^3]$, where $L$ is [integral](integral-split.md) minus [Simpson's rule](simpson-s-rule.md) and $(x-t)_+=\max(x-t,0)$ is the [positive part](positive-part-of-a-real-valued-function.md). Then $K(t)=-t^3(4-3t)/12$ for $0\leq t\leq1$ and $K(t)=-(2-t)^3(3t-2)/12$ for $1\leq t\leq2$. It is strictly negative inside the [interval](interval-mathematics.md) and has [integral](integral-split.md) $-1/15$. Thus

$$
L(f)=\frac1{3!}\int_0^2 K(t)f^{(4)}(t)\,dt,\qquad
|L(f)|\leq\frac{\|f^{(4)}\|_\infty}{90}.
$$

The [uniform norm](supremum-norm.md) $\|f^{(4)}\|_\infty$ bounds the fourth [derivative](derivative.md). The [polynomial](polynomial-split.md) $f(x)=x^4/24$ attains equality. Scaling to endpoint spacing $h$ multiplies the coefficient by $h^5$, giving the sharp single-panel bound $h^5\|f^{(4)}\|_\infty/90$. The normalized [Peano kernel](peano-kernel.md) is $K/3!$, so the external [factorial](factorial.md) must be omitted when using that normalization.

For the [exponential function](exponential-function.md) on $[0,1]$, $f^{(4)}(x)=e^x$, so $M=e$ and the bound is $e/(180n^4)$. Its leading actual [absolute error](absolute-error.md) is $(e-1)/(180n^4)$, smaller than the bound because a uniform upper bound on the fourth [derivative](derivative.md) does not use its variation across the [interval](interval-mathematics.md). The theorem bounds [truncation error](truncation-error.md) with exact [function evaluations](function-evaluation.md); sample errors and [roundoff error](round-off-error.md) are additional contributions, as described by [noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md).

## ↑ Ancestors (9)

1. [Composite Simpson's rule](composite-simpson-s-rule.md)
2. [Simpson's rule](simpson-s-rule.md)
3. [Quadrature rule](quadrature-rule.md)
4. [Numerical integration](numerical-integration-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Composite Simpson's rule](composite-simpson-s-rule.md)
