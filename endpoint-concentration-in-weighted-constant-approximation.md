# Endpoint concentration in weighted constant approximation

↑ **Parent:** [Weighted least squares](weighted-least-squares.md)

The constant minimizing $\int_{-1}^1x^{2n}(x^2-c)^2dx$ is the weighted mean

$$
c=\frac{\int_{-1}^1x^{2n+2}dx}{\int_{-1}^1x^{2n}dx}=\frac{2n+1}{2n+3}.
$$

This follows by differentiating the quadratic error or requiring the residual to be [orthogonal](orthogonal-vectors.md) to constants. The normalized weight $(2n+1)x^{2n}/2$ assigns mass $r^{2n+1}$ to $[-r,r]$ for every $0<r<1$. As $n$ increases it concentrates at the endpoints, where $x^2=1$, explaining the limiting best constant. Although the weight vanishes at zero, its integral against the square of a nonzero continuous function is positive, so the associated weighted [inner product](inner-product-split.md) is positive definite.

## ↑ Ancestors (8)

1. [Weighted least squares](weighted-least-squares.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/2/e/solution.md)
