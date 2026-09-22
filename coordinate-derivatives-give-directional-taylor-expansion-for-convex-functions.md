# Coordinate derivatives give directional Taylor expansion for convex functions

↑ **Parent:** [Convex function](convex-function.md)

Let $f$ be a finite [convex function](convex-function.md) on a neighbourhood of $x\in\mathbb R^d$, and suppose its first [partial derivatives](partial-derivative.md) exist at $x$. For any fixed [vector](vector.md) $h$, convexity gives

$$
f(x+th)\le\frac1d\sum_{i=1}^d f(x+dth_i e_i)
=f(x)+t\sum_{i=1}^d h_i\partial_i f(x)+o(t).
$$

The equality uses the one-dimensional first-order [Taylor expansion](taylor-expansion.md) along each coordinate line; no continuity of second [partial derivatives](partial-derivative.md) is assumed. Applying this upper bound to $-h$ and using $f(x)\le[f(x+th)+f(x-th)]/2$ gives the matching lower bound. Hence the displayed directional expansion holds. This supplies the expansion used in the [supporting inequality for a differentiable convex function](supporting-inequality-for-a-differentiable-convex-function.md) even when continuous second [partial derivatives](partial-derivative.md) have not been postulated.

## ↑ Ancestors (6)

1. [Convex function](convex-function.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/4/a/solution.md)
