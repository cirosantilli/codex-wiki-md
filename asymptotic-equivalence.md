# Asymptotic equivalence

↑ **Parent:** [Asymptotic analysis](asymptotic-analysis.md)

For [functions](function-split.md) with $g$ nonzero sufficiently near a specified [limit](limit-of-a-function.md),

$$
\boxed{f\sim g\quad\Longleftrightarrow\quad \frac{f}{g}\longrightarrow1.}
$$

The same definition applies to [sequences](sequence.md) $a_n\sim b_n$ as $n\to\infty$. Equivalently, $(f-g)/g\to0$: replacing $f$ by $g$ has a [relative error](relative-error.md) tending to zero, and the difference is $o(g)$ in [little o notation](little-o-notation.md). The [limit](limit-of-a-function.md) and reference scale are essential parts of the statement.

For example, $n^2+n\sim n^2$ because $(n^2+n)/n^2=1+1/n\to1$. Replacing the former by the latter gives [absolute error](absolute-error.md) $n$, which grows without bound. Thus [asymptotic equivalence](asymptotic-equivalence.md) controls a ratio, rather than requiring the [absolute error](absolute-error.md) to vanish. This distinction is crucial when approximating a rapidly growing [factorial](factorial.md) with [Stirling's formula](stirling-formula.md).

By contrast, $2n$ and $n$ have the same order in [big theta notation](big-theta-notation.md), but are not [asymptotically equivalent](asymptotic-equivalence.md): their ratio remains two. For positive [functions](function-split.md), [asymptotic equivalence](asymptotic-equivalence.md) gives both-sided constant bounds eventually, whereas constant bounds alone do not recover the leading coefficient.

<a id="image-local-exponential-approximation-relative-difference-tends-to-zero-and-absolute-error-is-quadratic"></a>
![](asymptotic-local-exponential-errors.png)

**[Figure 3](#image-local-exponential-approximation-relative-difference-tends-to-zero-and-absolute-error-is-quadratic). Local exponential approximation: relative difference tends to zero and absolute error is quadratic**.

For a local example with real $h$, the [exponential function](exponential-function.md) obeys $e^h-1\sim h$ as $h\to0$. The [Taylor theorem with Lagrange remainder](taylor-theorem-with-lagrange-remainder.md) gives

$$
e^h-1=h+\frac{e^\xi}{2}h^2,\qquad
|\xi|\le |h|.
$$

Thus for $|h|\le1$,

$$
|e^h-1-h|\le\frac e2 h^2.
$$

This states $e^h-1=h+O(h^2)$ in [big O notation](big-o-notation.md), and division by $h$ shows that the relative difference measured against $h$ vanishes. The diagram uses positive $h$; the bound is valid on both sides of zero. At $h=0.1$, the [absolute error](absolute-error.md) is approximately $0.00517092$ and the relative difference against $h$ is approximately $0.0517092$.

**Table of contents**

- [Asymptotic comparison of exponential functions](asymptotic-comparison-of-exponential-functions.md)
- [Stirling formula](stirling-formula.md)
  - [Robbins bounds for Stirling's formula](robbins-bounds-for-stirling-s-formula.md)
  - [Gaussian peak behind Stirling's formula](gaussian-peak-behind-stirling-s-formula.md)
  - [Stirling correction by Gaussian moments](stirling-correction-by-gaussian-moments.md)

## ↑ Ancestors (6)

1. [Asymptotic analysis](asymptotic-analysis.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Asymptotic analysis](asymptotic-analysis.md)
- [Asymptotic equivalence](asymptotic-equivalence.md)
- [Big O notation](big-o-notation.md)
- [Big theta notation](big-theta-notation.md)
- [Little o notation](little-o-notation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/30b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/32e/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/30e/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332/2/vi/solution.md)
- [Regular variation](regular-variation.md)
- [Second Chebyshev function](second-chebyshev-function.md)
- [Stirling formula](stirling-formula.md)
