# Weierstrass approximation theorem

↑ **Parent:** [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weierstrass_approximation_theorem)

Every [continuous](continuous-function.md) [real-valued function](real-valued-function.md) on a [compact interval](compact-interval.md) can be approximated by [polynomials](polynomial-split.md) with arbitrarily small error everywhere on the interval. More precisely, if $a<b$ and $f:[a,b]\to\mathbb R$ is [continuous](continuous-function.md), then for every $\varepsilon>0$ there is a [polynomial](polynomial-split.md) $p$ with

$$
\|f-p\|_\infty=\sup_{x\in[a,b]}|f(x)-p(x)|<\varepsilon.
$$

The error is measured in the [supremum norm](supremum-norm.md), so one approximation works at every point. The degenerate interval $a=b$ needs only a [constant function](constant-function.md). A change of variable $t=(x-a)/(b-a)$ reduces the nondegenerate case to $[0,1]$.[The Weierstrass approximation theorem, Theorem 0.3, printed p. 2: uniform polynomial approximation on the unit interval](the-weierstrass-approximation-theorem-georgia-tech-handout.md)

This is useful because a [polynomial](polynomial-split.md) is described by finitely many [coefficients](coefficient.md) and can be evaluated with [addition](addition.md) and [multiplication](multiplication.md). Its surprise is that the target need not be [differentiable](differentiable-function.md): the sharp corner of an [absolute value](absolute-value.md) function can be approximated by smooth [polynomials](polynomial-split.md). The [Bernstein approximation of a corner](bernstein-approximation-of-a-corner.md) below makes this visible. Approximating values, however, does not by itself approximate [derivatives](derivative.md); [Weierstrass approximation does not preserve derivatives](weierstrass-approximation-does-not-preserve-derivatives.md) gives a counterexample.

**Table of contents**

- [Weierstrass approximation does not preserve derivatives](weierstrass-approximation-does-not-preserve-derivatives.md)
- [Polynomial recurrence for the absolute value](polynomial-recurrence-for-the-absolute-value.md)
- [Bernstein polynomial](bernstein-polynomial.md)
  - [Bernstein approximation of a corner](bernstein-approximation-of-a-corner.md)
  - [Lipschitz error bound for Bernstein approximation](lipschitz-error-bound-for-bernstein-approximation.md)
  - [Bernstein polynomial degree preservation](bernstein-polynomial-degree-preservation.md)
  - [Derivatives of Bernstein polynomials](derivatives-of-bernstein-polynomials.md)
    - [Uniform convergence of Bernstein polynomial derivatives](uniform-convergence-of-bernstein-polynomial-derivatives.md)
  - [Bernstein falling-factorial identity](bernstein-falling-factorial-identity.md)
  - [Rounded Bernstein polynomial](rounded-bernstein-polynomial.md)
  - [Bernstein monomial recurrence](bernstein-monomial-recurrence.md)
  - [Inverse Bernstein approximation on a fixed-degree polynomial space](inverse-bernstein-approximation-on-a-fixed-degree-polynomial-space.md)
  - [Bernstein basis](bernstein-basis.md)
    - [Quadratic Bernstein coefficient bound](quadratic-bernstein-coefficient-bound.md)
    - [Positive Bernstein coefficients for a strictly positive polynomial](positive-bernstein-coefficients-for-a-strictly-positive-polynomial.md)
    - [Degree elevation of Bernstein coefficients](degree-elevation-of-bernstein-coefficients.md)

## ↑ Ancestors (6)

1. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (36)

- [Convergence of positive quadrature on continuous functions](convergence-of-positive-quadrature-on-continuous-functions.md)
- [Convergence of positive quadrature rules](convergence-of-positive-quadrature-rules.md)
- [Extension of approximation operators from a dense subspace](extension-of-approximation-operators-from-a-dense-subspace.md)
- [Interpolation nodes from best uniform approximation](interpolation-nodes-from-best-uniform-approximation.md)
- [Moment determinacy on a compact interval](moment-determinacy-on-a-compact-interval.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-69/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/18d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/2f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10/5/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-76/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/2f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/2f/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/2f/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-61/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/2i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/2f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/2f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105/1/2/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/11f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/11f/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/11f/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/11f/b/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/26k/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2/12f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/11h/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/17b/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/2f/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-358/2/b/solution.md)
- [Polynomial approximation](polynomial-approximation.md)
- [Polynomial recurrence for the absolute value](polynomial-recurrence-for-the-absolute-value.md)
