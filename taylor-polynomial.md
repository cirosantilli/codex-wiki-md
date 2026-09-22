# Taylor polynomial

↑ **Parent:** [Calculus](calculus-split.md)

A [Taylor polynomial](taylor-polynomial.md) replaces a [function](function-split.md) near a chosen point by a [polynomial](polynomial-split.md) with matching [derivatives](derivative.md). If $f$ has [derivatives](derivative.md) through order $n$ at $a$, define

$$
T_{n,a}(x)=\sum_{k=0}^n\frac{f^{(k)}(a)}{k!}(x-a)^k.
$$

The [factorial](factorial.md) denominator makes $T_{n,a}^{(j)}(a)=f^{(j)}(a)$ for $0\leq j\leq n$. This determines a unique [polynomial](polynomial-split.md) of [degree of a polynomial](degree-of-a-polynomial.md) at most $n$. Order zero matches the value, order one also matches the [tangent line](tangent-line.md), and order two also incorporates the second [derivative](derivative.md). Matching more local information is useful because [polynomials](polynomial-split.md) are easy to evaluate, differentiate, and integrate. The distinction between the finite [Taylor polynomial](taylor-polynomial.md) and the infinite [Taylor series](taylor-series.md) is developed in [OpenStax, Taylor and Maclaurin series](https://openstax.org/books/calculus-volume-2/pages/6-3-taylor-and-maclaurin-series).

For a computed example, let $f(x)=\sqrt{1+x}$ and expand at zero. Its first three [derivatives](derivative.md) give

$$
f(0)=1,\qquad f'(0)=\frac12,\qquad f''(0)=-\frac14,\qquad T_{2,0}(x)=1+\frac x2-\frac{x^2}8.
$$

At $x=0.1$, the linear approximation is $1.05$ and the quadratic approximation is $1.04875$, compared with $\sqrt{1.1}\approx1.048808848$. The quadratic correction captures the downward bending of the [square root](square-root.md) and reduces the absolute difference from about $0.00119115$ to $0.0000588482$.

<a id="image-matching-more-derivatives-improves-a-local-square-root-approximation-and-the-third-derivative-supplies-an-error-bound"></a>
![](taylor-square-root-approximation.png)

**[Figure 5](#image-matching-more-derivatives-improves-a-local-square-root-approximation-and-the-third-derivative-supplies-an-error-bound). Matching more derivatives improves a local square-root approximation, and the third derivative supplies an error bound**.

The [Taylor remainder](taylor-remainder.md) turns this convenient approximation into a controlled calculation. On $[0,0.1]$, $f'''(x)=3/[8(1+x)^{5/2}]$ is positive and at most $3/8$. The [Taylor theorem with Lagrange remainder](taylor-theorem-with-lagrange-remainder.md) therefore gives

$$
0<\sqrt{1.1}-1.04875\leq\frac{(3/8)(0.1)^3}{3!}=\frac1{16000}.
$$

Consequently **$1.04875<\sqrt{1.1}\leq1.0488125$** follows without using the displayed decimal evaluation as evidence. The [Taylor polynomial](taylor-polynomial.md) and the [Taylor remainder](taylor-remainder.md) play different roles: the former supplies an answer that is easy to compute, while the latter specifies what accuracy is justified. Farther from the expansion point, the same low-degree [polynomial](polynomial-split.md) need not remain accurate.

**Table of contents**

- [Multivariate Taylor polynomial](multivariate-taylor-polynomial.md)
  - [Second-order relative change of a monomial](second-order-relative-change-of-a-monomial.md)

## ↑ Ancestors (6)

1. [Calculus](calculus-split.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (47)

- [Blow-up compactness proof of an interior Schauder estimate](blow-up-compactness-proof-of-an-interior-schauder-estimate.md)
- [Hadamard finite-part reciprocal-power distribution](hadamard-finite-part-reciprocal-power-distribution.md)
- [Hölder-Taylor remainder bound](holder-taylor-remainder-bound.md)
- [Local linear approximation](local-linear-approximation.md)
- [Mean absolute error bound for local polynomial regression](mean-absolute-error-bound-for-local-polynomial-regression.md)
- [Mellin continuation of a nonprincipal Dirichlet L-function](mellin-continuation-of-a-nonprincipal-dirichlet-l-function.md)
- [Moment differentiation of the Fourier transform](moment-differentiation-of-the-fourier-transform.md)
- [Solution](past-exam-of-the-genetics-course-of-the-university-of-cambridge/2025/paper-4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-9/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-107/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/19d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-107/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-327/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/32a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-107/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/11/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/17/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/15/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/15/b/solution.md)
- [Peano zero](peano-zero.md)
- [Polynomial](polynomial-split.md)
- [Taylor normalization in elliptic blow-up arguments](taylor-normalization-in-elliptic-blow-up-arguments.md)
- [Taylor polynomial](taylor-polynomial.md)
- [Taylor remainder](taylor-remainder.md)
- [Taylor's theorem](taylor-s-theorem.md)
- [Taylor series](taylor-series.md)
- [Vanishing moment](vanishing-moment.md)
- [Vanishing moments and Fourier zeros](vanishing-moments-and-fourier-zeros.md)
- [Wavelet coefficient decay for Hölder functions](wavelet-coefficient-decay-for-holder-functions.md)
- [Wavelet polynomial annihilation](wavelet-polynomial-annihilation.md)
