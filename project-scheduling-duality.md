# Project scheduling duality

↑ **Parent:** [Critical path method](critical-path-method.md)

On the augmented precedence graph, the [linear programming](linear-programming.md) problem

$$
\min(t_{\mathrm{sink}}-t_{\mathrm{source}})
\quad\text{subject to}\quad t_j-t_i\geq\tau_i
$$

has dual $\max\sum_{i\to j}\tau_i f_{ij}$, with $f\geq0$ a unit source-to-sink flow. Equivalently, the dual is the negative of the optimal [uncapacitated minimum-cost flow](uncapacitated-minimum-cost-flow.md) value with arc costs $-\tau_i$. The flow selects a longest path, while the time variables provide a matching [weak duality](weak-duality.md) bound.

// Target: mathematical-optimization.bigb

**Table of contents**

- [Unit-flow certificate for project duration](unit-flow-certificate-for-project-duration.md)

## ↑ Ancestors (6)

1. [Critical path method](critical-path-method.md)
2. [Project scheduling](project-scheduling.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/2/solution.md)
