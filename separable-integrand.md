# Separable integrand

↑ **Parent:** [Numerical integration](numerical-integration-split.md)

An integrand is separable across coordinates when it factors as $g(x_1,\ldots,x_d)=\prod_{j=1}^dg_j(x_j)$. On a product domain, the [Fubini theorem](fubini-s-theorem.md) reduces its [integral](integral-split.md) to a product of one-dimensional [integrals](integral-split.md), provided the factors are [integrable](integrability.md); for nonnegative factors the [Tonelli theorem](tonelli-theorem.md) gives the extended-value version.

A finite sum of separable terms can likewise be integrated as a finite sum of products. For example,

$$
\int_{[0,1]^d}\sum_{i=1}^m e^{\|x-a_i\|^2}\,dx
=\sum_{i=1}^m\prod_{j=1}^d\int_0^1e^{(t-a_{ij})^2}\,dt.
$$

For fixed centres, the factors are smooth on compact [intervals](interval-mathematics.md). Repeated one-dimensional [composite Simpson's rule](composite-simpson-s-rule.md) refinements have fourth-order discretization error, avoiding the exponential tensor-grid cost of a generic $d$-dimensional rule. The numerical constants and possible [floating-point overflow](floating-point-overflow.md) still depend on the scale of the factors; separability removes a dimension-dependent combinatorial cost, not all conditioning difficulties.

## ↑ Ancestors (6)

1. [Numerical integration](numerical-integration-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [D](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/1/d.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/1/d/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/6/b/iv/solution.md)
