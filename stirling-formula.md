# Stirling formula

↑ **Parent:** [Asymptotic equivalence](asymptotic-equivalence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stirling_formula)

[Stirling's formula](stirling-formula.md) turns the long product defining a [factorial](factorial.md) into a short expression. For positive [integers](integer.md) $n$, put

$$
S_n=\sqrt{2\pi n}\left(\frac ne\right)^n.
$$

Then $n!\sim S_n$ as $n\to\infty$. This is [asymptotic equivalence](asymptotic-equivalence.md): $S_n/n!\to1$, so the [relative error](relative-error.md) tends to zero. It does not say that the [absolute error](absolute-error.md) tends to zero, and the formula is not an equality for finite $n$. The [Gamma function](gamma-function.md) extends this approximation beyond integer inputs. [NIST Digital Library of Mathematical Functions, §5.11: Gamma-function asymptotic expansions](https://dlmf.nist.gov/5.11)

For $n=10$,

$$
10!=3\,628\,800,\qquad S_{10}\simeq3\,598\,695.619,\qquad
\frac{S_{10}-10!}{10!}\simeq-0.00829596.
$$

The leading estimate is about $0.830\%$ low. Multiplying by the first correction factor gives

$$
S_{10}\left(1+\frac1{120}\right)\simeq3\,628\,684.749,
$$

which is about $0.003176\%$ low. The [Stirling correction by Gaussian moments](stirling-correction-by-gaussian-moments.md) explains why this factor is $1+1/(12n)$ rather than an arbitrary numerical adjustment.

<a id="image-relative-factorial-errors-shrink-faster-after-the-first-stirling-correction"></a>
![](stirling-factorial-relative-error.png)

**[Figure 4](#image-relative-factorial-errors-shrink-faster-after-the-first-stirling-correction). Relative factorial errors shrink faster after the first Stirling correction**. For each integer $1\leq n\leq100$, the curves compare $S_n$ and $S_n(1+1/(12n))$ with the exact [factorial](factorial.md). The vertical axis is the nonnegative [relative error](relative-error.md), on a logarithmic scale.

The usefulness is in ratios as well as in enormous numbers. Applying [Stirling's formula](stirling-formula.md) to the three [factorials](factorial.md) in a [central binomial coefficient](central-binomial-coefficient.md) gives

$$
\binom{2n}{n}\sim\frac{4^n}{\sqrt{\pi n}}.
$$

This counts the ways to choose exactly half of $2n$ objects. Equivalently, for $2n$ independent fair coin tosses, the [binomial distribution](binomial-distribution.md) assigns probability $\binom{2n}{n}/4^n\sim1/\sqrt{\pi n}$ to exactly $n$ heads. An exponentially large count becomes a simple probability scale after cancellation.

For numerical calculations, taking the [natural logarithm](natural-logarithm.md) yields

$$
\log(n!)=n\log n-n+\frac12\log(2\pi n)+r_n,
$$

where $r_n\to0$. Computing a [logarithm](logarithm.md) of a large [factorial](factorial.md) avoids representing the factorial itself. The [Robbins bounds for Stirling's formula](robbins-bounds-for-stirling-s-formula.md) give a finite-$n$ interval for this logarithmic remainder, rather than only a limiting statement.

The factor $\sqrt{2\pi n}$ is beautiful because a [Gaussian integral](gaussian-integral.md) lies behind a discrete product. The [Gaussian peak behind Stirling's formula](gaussian-peak-behind-stirling-s-formula.md) displays this connection through the [Gamma integral](gamma-integral.md) and [Laplace's method](laplace-s-method.md). A rigorous proof must also control the tails of the integral; the local expansion explains the geometry but is not by itself a complete proof.

James Stirling published _Methodus differentialis_ in 1730, a treatise on [summation](summation.md) and [interpolation](interpolation.md) of infinite [series](series-mathematics.md). This setting connects the formula with a practical calculation problem: taking [logarithms](logarithm.md) turns a long product into a [sum](sum.md), whose growth can be approximated. [James Stirling, Methodus differentialis (1730), digitized original and bibliographic record](https://commons.wikimedia.org/wiki/File:Methodus_differentialis,_sive_tractatus_de_summatione_et_interpolatione_serierum_infinitarum_(IA_10053880bsb).pdf)

**Table of contents**

- [Robbins bounds for Stirling's formula](robbins-bounds-for-stirling-s-formula.md)
- [Gaussian peak behind Stirling's formula](gaussian-peak-behind-stirling-s-formula.md)
- [Stirling correction by Gaussian moments](stirling-correction-by-gaussian-moments.md)

## ↑ Ancestors (7)

1. [Asymptotic equivalence](asymptotic-equivalence.md)
2. [Asymptotic analysis](asymptotic-analysis.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (38)

- [Entropy maximization for loss-network occupancy](entropy-maximization-for-loss-network-occupancy.md)
- [Factorial proof of Mertens first theorem](factorial-proof-of-mertens-first-theorem.md)
- [Independent spin-one-half two-level system](independent-spin-one-half-two-level-system.md)
- [Integrated Chebyshev sum](integrated-chebyshev-sum.md)
- [Order-one growth of the Riemann xi function](order-one-growth-of-the-riemann-xi-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-12/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-44/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-306/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/35a/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/3f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/3f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-150/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/36a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/7h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-150/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-150/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/37a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-201/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-336/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2/11f/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-208/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-109/4/iii/solution.md)
- [Stirling correction by Gaussian moments](stirling-correction-by-gaussian-moments.md)
- [Tree-component expectation in the Erdős-Rényi model](tree-component-expectation-in-the-erdos-renyi-model.md)
- [Vertical-strip factor in the Riemann zeta functional equation](vertical-strip-factor-in-the-riemann-zeta-functional-equation.md)
