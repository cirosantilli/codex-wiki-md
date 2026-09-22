# Numerical integration

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_integration)

[Numerical integration](numerical-integration-split.md) approximates a [definite integral](definite-integral.md) using finitely many sampled [function](function-split.md) values. For an [integrand](integrand.md) $f$ on a finite [interval](interval-mathematics.md) $[a,b]$, $a<b$, a [quadrature rule](quadrature-rule.md) has the form

$$
I(f)=\int_a^bf(x)\,dx,\qquad Q(f)=\sum_{j=1}^m w_jf(x_j)\approx I(f).
$$

The [quadrature nodes](quadrature-node.md) $x_j$ tell us where to evaluate $f$; the [quadrature weights](quadrature-weight.md) $w_j$ turn those values into an approximation to the accumulated signed area. The exact [definite integral](definite-integral.md) depends on the [integrand](integrand.md) throughout the [interval](interval-mathematics.md), whereas the [quadrature rule](quadrature-rule.md) sees only these samples. Integrating a chosen [interpolant](interpolant.md) exactly still generally approximates the original [integrand](integrand.md)'s [integral](integral-split.md).[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; Definition 5.6.1 and §5.6.1, equations 5.6.2–5.6.5: weighted samples and integration of an interpolant](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/5-6-numerical-integration.md)

The [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) evaluates $I(f)$ as $F(b)-F(a)$ when an [antiderivative](antiderivative.md) $F$ is available. [Numerical integration](numerical-integration-split.md) is useful when no convenient [antiderivative](antiderivative.md) is known, or each evaluation of the [integrand](integrand.md) requires an expensive computation. The task then becomes choosing informative [quadrature nodes](quadrature-node.md) and controlling the [quadrature error](quadrature-error.md) with as few evaluations as possible. Fixed data also permit a [quadrature rule](quadrature-rule.md), but refinement cannot supply new information between observations.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; Opening discussion, Example 5.6.1 and the paragraph following Definition 5.6.1: antiderivatives, numerical evaluation and fixed data](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/5-6-numerical-integration.md)

For an exact comparison, take the [polynomial](polynomial-split.md) $f(x)=x^2$ on $[0,1]$. Its [antiderivative](antiderivative.md) $x^3/3$ gives $I(f)=1/3$. On a [partition of an interval](partition-of-an-interval.md) into $n\geq1$ equal panels, the [composite midpoint quadrature rule](composite-midpoint-quadrature-rule.md) uses $n$ midpoint samples, each with [quadrature weight](quadrature-weight.md) $1/n$; the [composite trapezoidal rule](composite-trapezoidal-rule.md) uses $n+1$ endpoint samples, with outer [quadrature weights](quadrature-weight.md) $1/(2n)$ and interior [quadrature weights](quadrature-weight.md) $1/n$. The existing derivations under these two [quadrature rules](quadrature-rule.md) give

$$
M_n(f)=\frac13-\frac{1}{12n^2},\qquad T_n(f)=\frac13+\frac{1}{6n^2}.
$$

In particular, $M_1=1/4$ and $T_1=1/2$ already bracket $1/3$; two panels give $M_2=5/16$ and $T_2=3/8$. The [convex function](convex-function.md) $x^2$ explains the opposite signs. A midpoint [rectangle](rectangle.md) can cross the curve within its panel, so its total signed area, rather than pointwise ordering, determines the underestimate.

<a id="image-one-and-two-panels-for-numerical-integration-of-x-2-midpoint-and-endpoint-samples-with-their-quadrature-weights"></a>
![](quadrature-sample-weights-and-panels.png)

**[Figure 1](#image-one-and-two-panels-for-numerical-integration-of-x-2-midpoint-and-endpoint-samples-with-their-quadrature-weights). One and two panels for numerical integration of $x^2$: midpoint and endpoint samples with their quadrature weights**.

Define the signed [approximation error](approximation-error.md) as $E_n=Q_n(f)-I(f)$. In this example the [absolute errors](absolute-error.md) are $1/(12n^2)$ and $1/(6n^2)$: doubling $n$ reduces each by exactly four. A plot with both axes on a [logarithmic scale](logarithmic-scale.md) therefore has slope $-2$, expressing order two with respect to panel refinement. This is an exact calculation for this [polynomial](polynomial-split.md), including $n=1$, rather than an observed rate extrapolated from a few computed answers.

<a id="image-exact-absolute-errors-for-midpoint-and-trapezoidal-numerical-integration-of-x-2-slope-2-and-a-factor-four-reduction"></a>
![](quadrature-quadratic-errors-and-slope.png)

**[Figure 2](#image-exact-absolute-errors-for-midpoint-and-trapezoidal-numerical-integration-of-x-2-slope-2-and-a-factor-four-reduction). Exact absolute errors for midpoint and trapezoidal numerical integration of $x^2$: slope $-2$ and a factor-four reduction**.

For a general [integrand](integrand.md), the [composite midpoint quadrature rule](composite-midpoint-quadrature-rule.md) and [composite trapezoidal rule](composite-trapezoidal-rule.md) give second-order [quadrature error](quadrature-error.md) bounds when $f$ has two continuous [derivatives](derivative.md) on $[a,b]$ and a known bound on $|f''|$. These hypotheses describe behavior between samples. A formal error formula containing an unknown [derivative](derivative.md) is not a numerical accuracy certificate or a justified sample count. [Finite samples do not certify quadrature accuracy](finite-samples-do-not-certify-quadrature-accuracy.md) makes the missing information explicit. Errors in the evaluations and [roundoff error](round-off-error.md) must also be considered; [noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md) treats the former.

More elaborate choices exploit other information: [Gaussian quadrature](gaussian-quadrature.md) obtains high [polynomial](polynomial-split.md) exactness from carefully chosen [quadrature nodes](quadrature-node.md), and [Simpson's rule](simpson-s-rule.md) uses a quadratic [interpolant](interpolant.md). Adaptive [numerical integration](numerical-integration-split.md) compares approximations and concentrates samples where they disagree, often saving evaluations. Such a difference is an error estimate, not a certified bound without further assumptions: both approximations can miss the same feature.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §5.7.1, equation 5.7.4: a difference-based error estimate; §5.7.2: interval bisection; Example 5.7.2 and concluding discussion: requested accuracy is not guaranteed](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/5-7-adaptive-integration.md)

**Table of contents**

- [Finite samples do not certify quadrature accuracy](finite-samples-do-not-certify-quadrature-accuracy.md)
- [Boole's rule](boole-s-rule.md)
- [Quadrature rule](quadrature-rule.md)
  - [Quadrature node](quadrature-node.md)
  - [Quadrature weight](quadrature-weight.md)
  - [Degree of precision of a quadrature rule](degree-of-precision-of-a-quadrature-rule.md)
  - [Noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md)
  - [Newton-Cotes closed quadrature](newton-cotes-closed-quadrature.md)
  - [Simpson's rule](simpson-s-rule.md)
    - [Adaptive Simpson's method](adaptive-simpson-s-method.md)
    - [Cubic exactness of Simpson's rule](cubic-exactness-of-simpson-s-rule.md)
    - [Composite Simpson's rule](composite-simpson-s-rule.md)
      - [Error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md)
  - [Convergence of positive quadrature on continuous functions](convergence-of-positive-quadrature-on-continuous-functions.md)
  - [Nodal-polynomial criterion for quadrature exactness](nodal-polynomial-criterion-for-quadrature-exactness.md)
  - [Degree ceiling for quadrature exactness](degree-ceiling-for-quadrature-exactness.md)
  - [Positivity of quadrature weights from degree 2n exactness](positivity-of-quadrature-weights-from-degree-2n-exactness.md)
  - [Convergence of positive quadrature rules](convergence-of-positive-quadrature-rules.md)
  - [Moment matching](moment-matching.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)
- [Electrolysis](electrolysis.md)
- [Function evaluation](function-evaluation.md)
- [Galerkin orthogonality](galerkin-orthogonality.md)
- [Noise sensitivity of a quadrature rule](noise-sensitivity-of-a-quadrature-rule.md)
- [Numerical integration](numerical-integration-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/15f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219/2/d/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012/3/solution.md)
- [Pressure coefficient](pressure-coefficient.md)
- [Quadrature node](quadrature-node.md)
- [Quadrature rule](quadrature-rule.md)
- [Quadrature weight](quadrature-weight.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Twin paradox with finite acceleration](twin-paradox-with-finite-acceleration.md)
- [Worked supernova distance comparison](worked-supernova-distance-comparison.md)
