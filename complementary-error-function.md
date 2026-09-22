# Complementary error function

↑ **Parent:** [Error function](error-function.md)

The complementary error function describes the [Gaussian integral](gaussian-integral.md) area remaining beyond the endpoint. For a real $x$,

$$
\operatorname{erfc}(x)=1-\operatorname{erf}(x)=\frac{2}{\sqrt\pi}\int_x^\infty e^{-t^2}\,dt.
$$

It is an [entire function](entire-function.md) for complex arguments when defined by $1-\operatorname{erf}(z)$. On the [real line](real-line.md) it decreases from two to zero, with $\operatorname{erfc}(0)=1$ and $\operatorname{erfc}(-x)=2-\operatorname{erfc}(x)$.[§7.2(i), equation 7.2.2 and the entire-function statement](nist-digital-library-of-mathematical-functions/7-2-definitions.md)

For example, $\operatorname{erfc}(1)\approx0.157299$ is a sizeable tail, whereas $\operatorname{erfc}(8)\approx1.12243\times10^{-29}$ is extremely small. In the tested [floating-point arithmetic](floating-point-arithmetic-split.md), a direct evaluation of $1-\operatorname{erf}(8)$ gives zero because the computed [error function](error-function.md) has already rounded to one. Evaluating the [complementary error function](complementary-error-function.md) directly preserves this tail. It is the useful quantity in an upper-tail [normal distribution](normal-distribution.md) [probability](probability.md) and in the decaying side of an [error-function diffusion front](error-function-diffusion-front.md).

For large positive real $x$, the leading [asymptotic expansion](asymptotic-expansion-split.md) is

$$
\operatorname{erfc}(x)\sim\frac{e^{-x^2}}{\sqrt\pi x},\qquad x\to+\infty.
$$

The first corrections are $1-1/(2x^2)+3/(4x^4)-\cdots$ multiplying the leading term. This is an [asymptotic expansion](asymptotic-expansion-split.md), not an assertion that summing arbitrarily many terms converges at a fixed $x$.[§7.12(i), equation 7.12.1 and its real-axis remainder statement](nist-digital-library-of-mathematical-functions/7-12-asymptotic-expansions.md) The [complementary error function tail bound](complementary-error-function-tail-bound.md) provides finite-$x$ inequalities instead.

**Table of contents**

- [Complementary error function tail bound](complementary-error-function-tail-bound.md)
- [Faddeeva function](faddeeva-function.md)
  - [Gaussian pole integral](gaussian-pole-integral.md)

## ↑ Ancestors (9)

1. [Error function](error-function.md)
2. [Gaussian integral](gaussian-integral.md)
3. [Integral](integral-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Binary alloy Stefan similarity solution](binary-alloy-stefan-similarity-solution.md)
- [Complementary error function](complementary-error-function.md)
- [Constant-concentration inlet solution](constant-concentration-inlet-solution.md)
- [Constant-flux tracer inlet solution](constant-flux-tracer-inlet-solution.md)
- [Dilution function for a melting saline Stefan front](dilution-function-for-a-melting-saline-stefan-front.md)
- [Error function](error-function.md)
- [Error function and the normal distribution](error-function-and-the-normal-distribution.md)
- [Faddeeva function](faddeeva-function.md)
- [Gaussian integral](gaussian-integral.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-a/25/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-53/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-55/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-77/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/30a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-70/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-60/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-70/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-78/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-77/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/2/solution.md)
- [Salt-rejection function for a saline Stefan front](salt-rejection-function-for-a-saline-stefan-front.md)
