# Bernstein polynomial

↑ **Parent:** [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernstein_polynomial)

For a function $f:[0,1]\to\mathbb R$ and an [integer](integer-split.md) $n\geq1$, its [Bernstein polynomial](bernstein-polynomial.md) is

$$
B_nf(x)=\sum_{k=0}^n f(k/n)\binom nk x^k(1-x)^{n-k}
       =\mathbb E[f(K/n)],\qquad K\sim\operatorname{Bin}(n,x).
$$

The [Bernstein basis](bernstein-basis.md) supplies nonnegative weights whose sum is one. Equivalently, the weights are the [probabilities](probability.md) of a [binomial distribution](binomial-distribution.md), and the result is an [expected value](expected-value-split.md). At a given $x$, this averages the sampled values $f(k/n)$ with weights concentrated near $k/n=x$.[The Weierstrass approximation theorem, Lemmas 0.1–0.2 and Theorem 0.3, printed pp. 1–2: weights, binomial moments and polynomial construction](the-weierstrass-approximation-theorem-georgia-tech-handout.md)

The endpoints are exact: $B_nf(0)=f(0)$ and $B_nf(1)=f(1)$. Interior sampled points need not be interpolated. For example, [binomial distribution](binomial-distribution.md) moments give $B_n(x)=x$ and $B_n(x^2)=x^2+x(1-x)/n$. Thus every [affine function](affine-function.md) is reproduced exactly, whereas $x^2$ is generally changed. [Bernstein polynomial degree preservation](bernstein-polynomial-degree-preservation.md) is a statement about [degree of a polynomial](degree-of-a-polynomial.md), not equality of the entire [polynomial](polynomial-split.md).

For a [continuous](continuous-function.md) $f$, the [uniform continuity](uniform-continuity.md) of $f$ and the [variance](variance-split.md) $\operatorname{Var}(K/n)=x(1-x)/n\leq1/(4n)$ explain [uniform convergence](uniform-convergence.md). Split the [expected value](expected-value-split.md) of the error into $|K/n-x|<\delta$, where [uniform continuity](uniform-continuity.md) makes the change small, and its complement, whose [probability](probability.md) is at most $1/(4n\delta^2)$ by [Chebyshev's inequality](chebyshev-s-inequality.md). The [bounded function](bounded-function.md) $f$ bounds the remaining error. This proves convergence without assuming [differentiability](differentiability.md).

For $f\in C([0,1]^d)$, the tensor-product [Bernstein polynomial](bernstein-polynomial.md) is the [expected value](expected-value-split.md) of $f(X_1/n,\ldots,X_d/n)$ for [independent random variables](independent-random-variables.md) $X_j\sim\operatorname{Bin}(n,x_j)$. The same [uniform continuity](uniform-continuity.md) and coordinatewise [variance](variance-split.md) estimates give [uniform convergence](uniform-convergence.md) for each fixed finite $d$.

**Table of contents**

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

## ↑ Ancestors (7)

1. [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)
2. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (24)

- [Bernstein approximation of a corner](bernstein-approximation-of-a-corner.md)
- [Bernstein falling-factorial identity](bernstein-falling-factorial-identity.md)
- [Bernstein monomial recurrence](bernstein-monomial-recurrence.md)
- [Bernstein polynomial](bernstein-polynomial.md)
- [Extension of approximation operators from a dense subspace](extension-of-approximation-operators-from-a-dense-subspace.md)
- [Integer-coefficient polynomial approximation](integer-coefficient-polynomial-approximation.md)
- [Lipschitz error bound for Bernstein approximation](lipschitz-error-bound-for-bernstein-approximation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-69/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/12f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/11f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-339/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2/12f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/11g/i/solution.md)
- [Rounded Bernstein polynomial](rounded-bernstein-polynomial.md)
- [Uniform convergence of Bernstein polynomial derivatives](uniform-convergence-of-bernstein-polynomial-derivatives.md)
