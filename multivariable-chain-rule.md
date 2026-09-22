# Multivariable chain rule

↑ **Parent:** [Chain rule](chain-rule.md)

For [differentiable maps](differentiable-map.md) $f:\mathbb R^n\to\mathbb R^m$ and $g:\mathbb R^m\to\mathbb R^r$, the [multivariable chain rule](multivariable-chain-rule.md) multiplies their [Jacobian matrices](jacobian-matrix.md):

$$
J_{g\circ f}(x)=J_g(f(x))J_f(x).
$$

The outer $r\times m$ [matrix](matrix.md) multiplies the inner $m\times n$ [matrix](matrix.md), producing an $r\times n$ [matrix](matrix.md). This order records that the inner [linear map](linear-map.md) acts first. Componentwise, the [matrix multiplication](matrix-multiplication.md) sums the contributions of all intermediate coordinates. Existence of separate [partial derivatives](partial-derivative.md) alone is not the required [differentiability](differentiability.md) hypothesis.

**Table of contents**

- [Second derivatives under a two-variable coordinate change](second-derivatives-under-a-two-variable-coordinate-change.md)
- [Derivative along a curve](derivative-along-a-curve.md)
  - [Derivative of a vector field dotted with curve velocity](derivative-of-a-vector-field-dotted-with-curve-velocity.md)

## ↑ Ancestors (8)

1. [Chain rule](chain-rule.md)
2. [Derivative](derivative.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Derivative along a curve](derivative-along-a-curve.md)
- [Derivative of a vector field dotted with curve velocity](derivative-of-a-vector-field-dotted-with-curve-velocity.md)
- [Directional derivative](directional-derivative.md)
- [Gradient of a radial function](gradient-of-a-radial-function.md)
- [Logarithmic polar coordinate change](logarithmic-polar-coordinate-change.md)
- [Multivariable chain rule](multivariable-chain-rule.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018/section-b/b3/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2019/section-b/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/9/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/9/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/11/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/10/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/9/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1/18/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/18/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/19/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/16/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/18/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/17/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/13/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/12/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/19/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/17/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/14/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/14/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/14/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/16/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/20/a/solution.md)
- [Second derivatives under a two-variable coordinate change](second-derivatives-under-a-two-variable-coordinate-change.md)
- [Stationary points under an increasing outer function](stationary-points-under-an-increasing-outer-function.md)
- [Total derivative](total-derivative.md)
- [Volume derivative form of the heat-capacity difference](volume-derivative-form-of-the-heat-capacity-difference.md)
