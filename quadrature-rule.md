# Quadrature rule

↑ **Parent:** [Numerical integration](numerical-integration.md)

A [quadrature rule](quadrature-rule.md) approximates an [integral](integral.md) by a finite weighted sum of sampled [function](function-split.md) values:

$$
I_\rho(f)=\int_a^b\rho(x)f(x)\,dx\approx Q(f)=\sum_{i=1}^m w_i f(x_i).
$$

The [quadrature nodes](quadrature-node.md) $x_i$ specify where to sample, and the [quadrature weights](quadrature-weight.md) $w_i$ specify how much each sample contributes. The density $\rho(x)$ specifies the target [integral](integral.md), whereas the discrete [quadrature weights](quadrature-weight.md) belong to the approximation. Ordinary [numerical integration](numerical-integration.md) has $\rho=1$. [Gaussian quadrature](gaussian-quadrature.md) and the [midpoint quadrature rule](midpoint-quadrature-rule.md) choose interior [quadrature nodes](quadrature-node.md); the [trapezoidal rule](trapezoidal-rule.md) includes endpoints.[§3.5(iv), equation 3.5.15 and the following discussion of nodes and weights](nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-iv-interpolatory-quadrature-rules.md)

For ordinary [numerical integration](numerical-integration.md), exactness on the [constant function](constant-function.md) $1$ requires $\sum_iw_i=b-a$; exactness on $x$ additionally requires $\sum_iw_ix_i=(b^2-a^2)/2$. These two checks make the [quadrature rule](quadrature-rule.md) exact for every [affine function](affine-function.md). For example, both the [midpoint quadrature rule](midpoint-quadrature-rule.md) and [trapezoidal rule](trapezoidal-rule.md) give $6$ for $\int_0^2(2x+1)\,dx$. Testing progressively higher [polynomial degrees](degree-of-a-polynomial.md) defines the [degree of precision of a quadrature rule](degree-of-precision-of-a-quadrature-rule.md). Exactness describes a class of [integrands](integrand.md), rather than promising exact results for every [function](function-split.md).

[Composite midpoint quadrature rules](composite-midpoint-quadrature-rule.md) and [composite trapezoidal rules](composite-trapezoidal-rule.md) apply a simple [quadrature rule](quadrature-rule.md) on every panel of a [partition of an interval](partition-of-an-interval.md). This buys accuracy by shrinking the panels while keeping the elementary formula fixed. For [continuous functions](continuous-function.md) sampled exactly, their [quadrature errors](quadrature-error.md) tend to zero as the largest panel width tends to zero. The familiar second-order bounds require stronger assumptions about [derivatives](derivative.md). The signed [approximation error](approximation-error.md) used here is $Q(f)-I_\rho(f)$; some sources define [quadrature error](quadrature-error.md) with the opposite sign, so the convention must accompany any formula.

**Table of contents**

- [Quadrature node](quadrature-node.md)
- [Quadrature weight](quadrature-weight.md)
- [Degree of precision of a quadrature rule](degree-of-precision-of-a-quadrature-rule.md)
- [Noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md)
- [Newton-Cotes closed quadrature](newton-cotes-closed-quadrature.md)
- [Simpson's rule](simpson-s-rule.md)
- [Convergence of positive quadrature on continuous functions](convergence-of-positive-quadrature-on-continuous-functions.md)
- [Nodal-polynomial criterion for quadrature exactness](nodal-polynomial-criterion-for-quadrature-exactness.md)
- [Degree ceiling for quadrature exactness](degree-ceiling-for-quadrature-exactness.md)
- [Positivity of quadrature weights from degree 2n exactness](positivity-of-quadrature-weights-from-degree-2n-exactness.md)
- [Convergence of positive quadrature rules](convergence-of-positive-quadrature-rules.md)
- [Moment matching](moment-matching.md)

## ↑ Ancestors (6)

1. [Numerical integration](numerical-integration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Convergence of positive quadrature on continuous functions](convergence-of-positive-quadrature-on-continuous-functions.md)
- [Gaussian quadrature](gaussian-quadrature.md)
- [Lagrange polynomial](lagrange-polynomial.md)
- [Newton-Cotes closed quadrature](newton-cotes-closed-quadrature.md)
- [Nodal-polynomial criterion for quadrature exactness](nodal-polynomial-criterion-for-quadrature-exactness.md)
- [Noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/18c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341/section-a/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/17b/b/solution.md)
- [Polynomial interpolation](polynomial-interpolation.md)
- [Quadrature node](quadrature-node.md)
- [Quadrature rule](quadrature-rule.md)
- [Quadrature weight](quadrature-weight.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Trapezoidal rule](trapezoidal-rule.md)
