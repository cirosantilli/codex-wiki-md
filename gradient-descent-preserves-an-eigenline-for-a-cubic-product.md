# Gradient descent preserves an eigenline for a cubic product

↑ **Parent:** [Gradient descent](gradient-descent-split.md)

Let $A$ be real symmetric, let $b$ be a unit [eigenvector](eigenvector.md) satisfying $Ab=\lambda b$, and use scalar [step sizes](step-size.md) $\alpha_n$. The [gradient](gradient.md) of the displayed [cubic polynomial](cubic-polynomial.md) [function](function-split.md) is

$$
\nabla h(x)=2(x^Tb)Ax+(x^TAx)b.
$$

On the [eigenline](eigenline.md), $\nabla h(tb)=3\lambda t^2b$, so a [gradient descent](gradient-descent-split.md) update remains on that same line and obeys the scalar recurrence in the title. Induction proves invariance for every iterate starting on the line, including an iterate that reaches zero. This is a statement about the geometry of the updates, not a convergence theorem: when $\lambda\ne0$, the restriction $h(tb)=\lambda t^3$ is unbounded below in one direction.

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/5/c/iii/solution.md)
