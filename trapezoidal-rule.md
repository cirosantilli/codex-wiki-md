# Trapezoidal rule

↑ **Parent:** [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trapezoidal_rule)

As a [quadrature rule](quadrature-rule.md), the [trapezoidal rule](trapezoidal-rule.md) replaces an [integrand](integrand.md) by the [linear interpolation](linear-interpolation.md) joining its two endpoint values:

$$
I(f)=\int_a^bf(x)\,dx\approx T(f)=\frac{b-a}{2}\bigl(f(a)+f(b)\bigr),\qquad a<b.
$$

For nonnegative endpoint values, this is the area of a [trapezoid](trapezoid.md); in general it is a signed area. The [quadrature nodes](quadrature-node.md) are $a,b$, each with [quadrature weight](quadrature-weight.md) $(b-a)/2$. Unlike the [midpoint quadrature rule](midpoint-quadrature-rule.md), it uses endpoint samples, which can be reused between adjacent panels.

Every [affine function](affine-function.md) $f(x)=\alpha x+\beta$ agrees with its [linear interpolation](linear-interpolation.md), so the [trapezoidal rule](trapezoidal-rule.md) integrates it exactly. On $[0,2]$, $f(x)=2x+1$ gives $T(f)=(2/2)(1+5)=6=I(f)$. On $[0,1]$, the [polynomial](polynomial-split.md) $f(x)=x^2$ instead gives $T(f)=1/2$, exceeding $I(f)=1/3$ by $1/6$. Its [degree of precision of a quadrature rule](degree-of-precision-of-a-quadrature-rule.md) is exactly one.

If $f\in C^2[a,b]$, its signed [approximation error](approximation-error.md) satisfies

$$
T(f)-I(f)=\frac{(b-a)^3}{12}f''(\xi_T),\qquad a<\xi_T<b.
$$

A [convex function](convex-function.md) lies below its endpoint chord, so the [trapezoidal rule](trapezoidal-rule.md) overestimates its [integral](integral-split.md); a [concave function](concave-function.md) gives the reverse inequality. The error formula assumes that the second [derivative](derivative.md) exists and is a [continuous function](continuous-function.md) throughout the closed interval.[§3.5(i), equation 3.5.1 and its C² hypothesis; the source writes integral minus rule](nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-i-trapezoidal-rules.md) A short derivation is the identity

$$
T(f)-I(f)=\frac12\int_a^b(t-a)(b-t)f''(t)\,dt,
$$

obtained by two [integrations by parts](integration-by-parts.md). The nonnegative [Peano kernel](peano-kernel.md) has [integral](integral-split.md) $(b-a)^3/12$, and the [weighted mean value theorem for integrals](weighted-mean-value-theorem-for-integrals.md) gives the formula.

The [trapezoidal rule](trapezoidal-rule.md) for an [ordinary differential equation](ordinary-differential-equation.md) averages [vector fields](vector-field.md) at the old and new states and is [A-stable](a-stability.md).

This time-stepping use applies the same [trapezoidal rule](trapezoidal-rule.md) to the [integral](integral-split.md) of the [derivative](derivative.md) in an [ordinary differential equation](ordinary-differential-equation.md). That connection explains its place under [implicit Runge-Kutta methods](implicit-runge-kutta-method.md); its quadrature behavior and the nonlinear issue in [trapezoidal rule fails B-stability](trapezoidal-rule-fails-b-stability.md) concern different uses of the same endpoint averaging.

**Table of contents**

- [Composite trapezoidal rule](composite-trapezoidal-rule.md)
- [Trapezoidal rule fails B-stability](trapezoidal-rule-fails-b-stability.md)

## ↑ Ancestors (7)

1. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
2. [Runge-Kutta method](runge-kutta-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (36)

- [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)
- [Composite trapezoidal rule](composite-trapezoidal-rule.md)
- [Crank-Nicolson method](crank-nicolson-method.md)
- [Finite samples do not certify quadrature accuracy](finite-samples-do-not-certify-quadrature-accuracy.md)
- [Heun's method](heun-s-method.md)
- [Lift (force)](lift-force-split.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/7/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/7/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/38c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/17c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341/section-a/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341/section-a/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341/5/b/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341/6/solution.md)
- [Quadrature rule](quadrature-rule.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Theta method](theta-method.md)
- [Trapezoidal-BDF two-step family](trapezoidal-bdf-two-step-family.md)
- [Trapezoidal rule](trapezoidal-rule.md)
- [Trapezoidal rule fails B-stability](trapezoidal-rule-fails-b-stability.md)
- [Two-step family with a third-order member](two-step-family-with-a-third-order-member.md)
