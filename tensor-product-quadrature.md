# Tensor-product quadrature

↑ **Parent:** [Numerical integration](numerical-integration-split.md)

On a product domain, apply a one-dimensional [quadrature rule](quadrature-rule.md) independently in each coordinate. The resulting [quadrature nodes](quadrature-node.md) form a product grid and the [quadrature weights](quadrature-weight.md) multiply. With $m$ subdivisions per direction in fixed dimension $d$, the evaluation count is $N=O(m^d)$. If the one-dimensional rule has error $O(m^{-p})$, uniformly for the required coordinate slices, and its weight sums are bounded, telescoping the $d$ integration operators against their quadrature operators gives total error $O(m^{-p})=O(N^{-p/d})$. Thus [composite Simpson's rule](composite-simpson-s-rule.md) has $p=4$ for sufficiently smooth integrands, but loses efficiency as $d$ increases.

## ↑ Ancestors (6)

1. [Numerical integration](numerical-integration-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [D](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/1/d.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/1/d/i/solution.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2017/1/d/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/continuous-mathematics/5/a/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/continuous-mathematics/5/a/v/solution.md)
