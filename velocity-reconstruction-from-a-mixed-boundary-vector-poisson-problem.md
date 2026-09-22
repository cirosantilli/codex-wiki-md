# Velocity reconstruction from a mixed-boundary vector Poisson problem

↑ **Parent:** [Vector potential](vector-potential.md)

Let $D$ be bounded, connected and [simply connected](simply-connected-space.md), and let $u$ be a smooth [divergence](divergence.md)-free field. Suppose a sufficiently smooth vector field $A$ satisfies the displayed Poisson and [boundary conditions](boundary-condition.md). [Divergence](divergence.md) gives $\Delta\operatorname{div}A=0$ with zero [boundary](boundary-of-a-set.md) value, so harmonic uniqueness gives $\operatorname{div}A=0$. The vector Laplacian identity then implies $\nabla\times(\nabla\times A-u)=0$.

On a [simply connected](simply-connected-space.md) domain, define a [scalar potential](scalar-potential.md) by integrating this [curl](curl.md)-free difference along a path from a fixed point. Vanishing circulation around contractible loops proves path independence. Thus the difference is $\nabla\chi$; its [divergence](divergence.md) and [boundary](boundary-of-a-set.md) normal component give $\Delta\chi=0$ and $\partial_n\chi=0$. Green's identity yields $\int_D|\nabla\chi|^2=0$, proving the reconstruction. Additional conditions on $A$ can specify its own [boundary](boundary-of-a-set.md) problem; the argument assumes its existence and proves that its [curl](curl.md) is exactly $u$. Simple connectivity is essential for eliminating possible non-[gradient](gradient.md) harmonic circulation fields.

## ↑ Ancestors (10)

1. [Vector potential](vector-potential.md)
2. [Curl](curl.md)
3. [Vector calculus](vector-calculus.md)
4. [Multivariable calculus](multivariable-calculus-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-topics-in-fluid-mechanics-course-of-the-university-of-oxford/2008/1/solution.md)
