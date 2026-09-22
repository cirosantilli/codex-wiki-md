<h1 id="simpson-s-rule">Simpson's rule</h1>

↑ **Parent:** [Quadrature rule](quadrature-rule.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simpson's_rule)

[Simpson's rule](simpson-s-rule.md) approximates a [definite integral](definite-integral.md) by integrating the [quadratic polynomial](quadratic-polynomial.md) obtained by [polynomial interpolation](polynomial-interpolation.md) at two endpoints and their [midpoint](midpoint.md). For an [interval](interval-mathematics.md) $[a,b]$ with $a<b$, write $m=(a+b)/2$ and $h=(b-a)/2$. The three [quadrature nodes](quadrature-node.md) are $a,m,b$, and the [quadrature rule](quadrature-rule.md) is

$$
S(f)=\frac h3\bigl[f(a)+4f(m)+f(b)\bigr].
$$

Thus its [quadrature weights](quadrature-weight.md) are $h/3,4h/3,h/3$. Their sum is $2h=b-a$, as required for exactness on [constant functions](constant-function.md). This is the three-node [Newton-Cotes closed quadrature](newton-cotes-closed-quadrature.md); its [degree of precision of a quadrature rule](degree-of-precision-of-a-quadrature-rule.md) is three, even though the interpolating [polynomial](polynomial-split.md) has [polynomial degree](degree-of-a-polynomial.md) at most two.[NIST Digital Library of Mathematical Functions; §3.5(ii), equation 3.5.6: elementary Simpson rule and its fourth-derivative remainder](nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-ii-simpson%E2%80%99s-rule.md)

For an original worked example, take the [cubic polynomial](cubic-polynomial.md) $f(x)=x^3-2x+4$ on the [interval](interval-mathematics.md) $[-1,2]$. Here $m=1/2$ and $h=3/2$, so the [function evaluations](function-evaluation.md) give

$$
f(-1)=5,\qquad f(1/2)=\frac{25}{8}=3.125,\qquad f(2)=8.
$$

[Simpson's rule](simpson-s-rule.md) gives

$$
S(f)=\frac12\left(5+4\cdot\frac{25}{8}+8\right)=\frac{51}{4}=12.75.
$$

An [antiderivative](antiderivative.md) supplies an independent exact [definite integral](definite-integral.md):

$$
\int_{-1}^{2}(x^3-2x+4)\,dx
=\left[\frac{x^4}{4}-x^2+4x\right]_{-1}^{2}
=\frac{51}{4}.
$$

The [quadratic polynomial](quadratic-polynomial.md) through the same [quadrature nodes](quadrature-node.md) is $p_2(x)=\tfrac32x^2-\tfrac12x+3$. It differs from $f$ between the [quadrature nodes](quadrature-node.md), but its [definite integral](definite-integral.md) agrees exactly. The picture shows why: the signed [polynomial interpolation error](polynomial-interpolation-error.md) has two lobes with opposite [integrals](integral-split.md).

<a id="image-an-original-cubic-and-its-quadratic-interpolant-have-the-same-integral-because-the-two-interpolation-error-lobes-have-signed-integrals-plus-and-minus-81-over-64"></a>
![](simpson-cubic-error-cancellation.png)

**[Figure 3](#image-an-original-cubic-and-its-quadratic-interpolant-have-the-same-integral-because-the-two-interpolation-error-lobes-have-signed-integrals-plus-and-minus-81-over-64). An original cubic and its quadratic interpolant have the same integral because the two interpolation-error lobes have signed integrals plus and minus 81 over 64**.

Three [function evaluations](function-evaluation.md) therefore capture more information about an [integral](integral-split.md) than about the whole [function](function-split.md). When an [antiderivative](antiderivative.md) is unavailable, [composite Simpson's rule](composite-simpson-s-rule.md) repeats this inexpensive local construction over a [partition of an interval](partition-of-an-interval.md). For a sufficiently smooth [function](function-split.md), halving the node spacing reduces its [truncation error](truncation-error.md) by approximately a factor of sixteen.

**Table of contents**

- [Adaptive Simpson's method](adaptive-simpson-s-method.md)
- [Cubic exactness of Simpson's rule](cubic-exactness-of-simpson-s-rule.md)
- [Composite Simpson's rule](composite-simpson-s-rule.md)
  - [Error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md)

## ↑ Ancestors (7)

1. [Quadrature rule](quadrature-rule.md)
2. [Numerical integration](numerical-integration-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Composite Simpson's rule](composite-simpson-s-rule.md)
- [Cubic exactness of Simpson's rule](cubic-exactness-of-simpson-s-rule.md)
- [Error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md)
- [Numerical integration](numerical-integration-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/19c/solution.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Simpson's rule](simpson-s-rule.md)
