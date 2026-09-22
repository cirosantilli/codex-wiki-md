# Krivine rounding scheme

↑ **Parent:** [Gaussian hyperplane rounding](gaussian-hyperplane-rounding.md)

For a bipartite [elliptope](elliptope.md) [matrix](matrix.md) $X$, put $t=\log(1+\sqrt2)$ and apply $\sinh(tx)$ within the two diagonal blocks and $\sin(tx)$ across them. Matching absolute [power series](power-series.md) [coefficients](coefficient.md) give a [positive semidefinite matrix](positive-semidefinite-matrix.md) by [coefficient-dominated entrywise positivity](coefficient-dominated-entrywise-positivity.md), while $\sinh t=1$ gives unit diagonal. [Gaussian hyperplane rounding](gaussian-hyperplane-rounding.md) then turns each cross-block [correlation coefficient](pearson-correlation-coefficient.md) into $(2/\pi)\arcsin(\sin(tX_{ij}))=(2t/\pi)X_{ij}$ because $t<\pi/2$. The zero diagonal blocks of the bipartite objective eliminate every other contribution.

**Table of contents**

- [Bipartite sign rounding bound](bipartite-sign-rounding-bound.md)
- [Krivine rounding constant](krivine-rounding-constant.md)

## ↑ Ancestors (6)

1. [Gaussian hyperplane rounding](gaussian-hyperplane-rounding.md)
2. [Randomized rounding](randomized-rounding.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Bipartite binary quadratic optimization](bipartite-binary-quadratic-optimization.md)
- [Bipartite sign rounding bound](bipartite-sign-rounding-bound.md)
- [Krivine rounding constant](krivine-rounding-constant.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-339/2/e/solution.md)
