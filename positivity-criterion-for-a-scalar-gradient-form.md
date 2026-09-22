# Positivity criterion for a scalar gradient form

↑ **Parent:** [Bounded bilinear form](bounded-bilinear-form.md)

Let $c$ be a bounded real measurable coefficient on an open set. Nonnegativity of $c$ clearly makes its gradient form nonnegative. Conversely, if $c<0$ on a set of positive measure, choose an interior [Lebesgue point](lebesgue-point.md) $x_0$ where $c(x_0)<0$. For a nonconstant compactly supported smooth function $\psi$, set $v_\varepsilon(x)=\varepsilon\psi((x-x_0)/\varepsilon)$. Change variables and use the [Lebesgue differentiation theorem](lebesgue-differentiation-theorem.md) to obtain $\varepsilon^{-n}\int c|\nabla v_\varepsilon|^2\to c(x_0)\int|\nabla\psi|^2<0$, a contradiction. Thus the linear operator represented by $a(u,v)=\int c\nabla u\cdot\nabla v$ is monotone exactly when $c\geq0$ almost everywhere.

## ↑ Ancestors (7)

1. [Bounded bilinear form](bounded-bilinear-form.md)
2. [Bilinear form](bilinear-form-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-methods-of-applied-functional-analysis-course-of-the-university-of-oxford/2010/b/6/c/i/solution.md)
