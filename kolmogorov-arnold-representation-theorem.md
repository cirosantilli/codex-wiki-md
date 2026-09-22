# Kolmogorov-Arnold representation theorem

↑ **Parent:** [Uniform approximation](uniform-approximation-split.md)

Every real [continuous function](continuous-function.md) on a compact square can be represented as $\sum_{q=1}^5G_q(a_q(x)+b_q(y))$, with continuous one-variable functions and fixed inner functions $a_q,b_q$ independent of the represented function. [Grid-separated additive coordinates](grid-separated-additive-coordinates.md) give the inner functions. For a residual $r$ of norm $M$, assign $r$ at a sample point divided by three to each separated rectangle image, and continuously interpolate between images. Each point lies in at least three rectangles, so if $k\in\{3,4,5\}$ summands are accurate, the error is at most $[|1-k/3|+(5-k)/3]M+5\eta/3=2M/3+5\eta/3$. Choose oscillation $\eta\le M/10$ to obtain contraction $5/6$. Iteration gives outer functions by [uniform convergence](uniform-convergence.md) of corrections bounded by $M(5/6)^j/3$. [Whole-plane reduction for continuous superposition](whole-plane-reduction-for-continuous-superposition.md) removes compactness of the original domain without assuming boundedness of the original function.

**Table of contents**

- [Whole-plane reduction for continuous superposition](whole-plane-reduction-for-continuous-superposition.md)
- [Grid-separated additive coordinates](grid-separated-additive-coordinates.md)

## ↑ Ancestors (5)

1. [Uniform approximation](uniform-approximation-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-8/1/solution.md)
- [Whole-plane reduction for continuous superposition](whole-plane-reduction-for-continuous-superposition.md)
