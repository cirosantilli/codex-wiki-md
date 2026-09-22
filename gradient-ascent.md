# Gradient ascent

↑ **Parent:** [Gradient descent](gradient-descent.md)

[Gradient ascent](gradient-ascent.md) seeks a maximum by stepping along the [gradient](gradient.md) of a differentiable objective. It is [gradient descent](gradient-descent.md) applied to $-J$. Taylor expansion gives $J(x+\eta\nabla J)=J(x)+\eta\|\nabla J\|^2+O(\eta^2)$, so sufficiently small positive steps improve the objective when the [gradient](gradient.md) is nonzero. Line search, projection onto admissible controls, and noise-aware [gradient](gradient.md) estimates are common practical modifications; a local stationary result need not be globally optimal.

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gradient ascent](gradient-ascent.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/3/b/solution.md)
