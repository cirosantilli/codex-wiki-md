<h1 id="holder-s-inequality">Hölder's inequality</h1>

↑ **Parent:** [Lp norm](lp-norm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hölder's_inequality)

[Hölder's inequality](holder-s-inequality.md) controls a product using separate information about its two factors. If one factor is large on part of a domain, the other factor's complementary [Lp norm](lp-norm.md) limits how much their product can accumulate there. The same statement bounds finite [sums](sum.md), [integrals](integral-split.md) and [expected values](expected-value-split.md); no [independence](independent-random-variables.md) is required in the probabilistic version.

Let $p,q\in[1,\infty]$ be [conjugate exponents](conjugate-exponents.md), meaning

$$
\frac1p+\frac1q=1,\qquad\frac1\infty=0.
$$

On a [measure space](measure-space.md), if $f\in L^p$ and $g\in L^q$, then $fg\in L^1$ and

$$
\boxed{\int |fg|\,d\mu\leq\lVert f\rVert_p\lVert g\rVert_q.}
$$

Here the [Lp norms](lp-norm.md) are finite; at exponent $\infty$ the norm uses the [essential supremum](essential-supremum.md). For a finite [vector](vector.md), integration with [counting measure](counting-measure.md) gives

$$
\left|\sum_i x_i y_i\right|\leq\sum_i|x_i y_i|
\leq\left(\sum_i|x_i|^p\right)^{1/p}
\left(\sum_i|y_i|^q\right)^{1/q},\qquad 1<p,q<\infty.
$$

The first step is the [triangle inequality](triangle-inequality.md); the second is [Hölder's inequality](holder-s-inequality.md).[NIST Digital Library of Mathematical Functions, §1.7(i)–(ii), equations 1.7.2 and 1.7.5 and the accompanying equality statements](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

For finite [vectors](vector.md), the endpoint case $p=1$, $q=\infty$ is $|x^Ty|\leq\lVert x\rVert_1\lVert y\rVert_\infty$: bound every $|y_i|$ by its [maximum](maximum-of-a-subset-of-a-total-order.md), then sum the $|x_i|$. Swapping the factors gives the other endpoint. The choice $p=q=2$ gives the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md).

**Table of contents**

- [Conjugate exponent](conjugate-exponent.md)
- [Finite-vector example of Hölder's inequality](finite-vector-example-of-holder-s-inequality.md)
- [Equality in Hölder's inequality](equality-in-holder-s-inequality.md)
- [Probabilistic use of Hölder's inequality](probabilistic-use-of-holder-s-inequality.md)
- [History of Hölder's inequality](history-of-holder-s-inequality.md)

## ↑ Ancestors (6)

1. [Lp norm](lp-norm.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (48)

- [Closed-hyperplane proof of Lp duality](closed-hyperplane-proof-of-lp-duality.md)
- [Compact L2 potential perturbation of the Dirichlet Laplacian](compact-l2-potential-perturbation-of-the-dirichlet-laplacian.md)
- [Equality in Hölder's inequality](equality-in-holder-s-inequality.md)
- [Finite-vector example of Hölder's inequality](finite-vector-example-of-holder-s-inequality.md)
- [Fourier stability of a linear configuration count](fourier-stability-of-a-linear-configuration-count.md)
- [Functional Loomis-Whitney inequality](functional-loomis-whitney-inequality.md)
- [Hardy's integral inequality](hardy-s-integral-inequality.md)
- [Hedberg inequality](hedberg-inequality.md)
- [Hölder's inequality](holder-s-inequality.md)
- [Lp norm](lp-norm.md)
- [Minkowski inequality](minkowski-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-8/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-8/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-8/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-7/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/21f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-10/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-5/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/22f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-13/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-13/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/22h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/22h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/23j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/22f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/24j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/23f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-109/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-129/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-117/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/3/b/solution.md)
- [Proof outline of Hardy's integral inequality](proof-outline-of-hardy-s-integral-inequality.md)
- [Section induction for the Talagrand exponential moment](section-induction-for-the-talagrand-exponential-moment.md)
- [Uniform covers theorem](uniform-covers-theorem.md)
- [Upper maximal moment bound for a continuous local martingale](upper-maximal-moment-bound-for-a-continuous-local-martingale.md)
