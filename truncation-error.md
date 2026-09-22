# Truncation error

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Truncation_error)

[Truncation error](truncation-error.md) is introduced by replacing an exact operation with a finite approximation. It remains even when all arithmetic is exact. For $f(x)=x^2$, the forward [finite difference](finite-difference-split.md) for its [derivative](derivative.md) at $x=1$ gives

$$
\frac{f(1+h)-f(1)}h=2+h,\qquad f'(1)=2.
$$

Thus the [truncation error](truncation-error.md) is exactly $h$: $h=0.1$ gives $2.1$ and $h=0.01$ gives $2.01$. In finite precision, however, the numerator subtracts nearly equal values, and their [roundoff error](round-off-error.md) can be amplified by division by $h$. For smooth data with bounded evaluation errors of scale $u$, a typical bound has competing terms $C_1h+C_2u/h$. Smaller $h$ reduces the first term and increases the second; with fixed positive constants the balancing scale is $h\sim\sqrt u$. This is why blindly refining a [finite difference](finite-difference-split.md) eventually stops improving it.

**Table of contents**

- [Series truncation error](series-truncation-error.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Composite Simpson's rule](composite-simpson-s-rule.md)
- [Error bound for composite Simpson's rule](error-bound-for-composite-simpson-s-rule.md)
- [Noise amplification by differentiation of a linear interpolant](noise-amplification-by-differentiation-of-a-linear-interpolant.md)
- [Numerical analysis](numerical-analysis-split.md)
- [Numerical differentiation](numerical-differentiation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/39a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/5c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/5c/c/solution.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2015/1/d/solution.md)
- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2010/b/5/b/solution.md)
- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2010/b/5/d/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/1/c/solution.md)
- [Solution](past-exam-of-the-short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2019/s31/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/5/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/continuous-mathematics/5/d/solution.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Round-off error](round-off-error.md)
- [Series truncation error](series-truncation-error.md)
- [Simpson's rule](simpson-s-rule.md)
- [Step-size choice for a noisy central derivative](step-size-choice-for-a-noisy-central-derivative.md)
- [Truncation error](truncation-error.md)
