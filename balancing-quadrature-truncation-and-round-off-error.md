# Balancing quadrature truncation and round-off error

↑ **Parent:** [Numerical integration](numerical-integration-split.md)

If a [quadrature](phase-quadrature.md) error bound is $C n^{-p}$ and the relevant numerical resolution is $\delta$, equating these scales gives an estimate of the strip count beyond which that truncation guarantee reaches the [rounding](rounding.md) scale. For the [composite Simpson's rule](composite-simpson-s-rule.md), $p=4$. This estimate is useful for choosing a sensible order of magnitude, but a worst-case bound need not equal the actual [quadrature](phase-quadrature.md) error.

For a normal [floating-point number](floating-point-number.md) in base two, the spacing depends on the exponent of the result; half the spacing is a natural final-storage [rounding](rounding.md) scale. [Machine epsilon](machine-epsilon.md) instead measures the gap above one. [Function](function-split.md)-evaluation errors, accumulation of summation error, cancellation, and the arithmetic used for the nodes can impose an earlier practical accuracy limit. Thus final storage precision alone cannot give a universal optimal strip count.

## ↑ Ancestors (6)

1. [Numerical integration](numerical-integration-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/6/d/solution.md)
