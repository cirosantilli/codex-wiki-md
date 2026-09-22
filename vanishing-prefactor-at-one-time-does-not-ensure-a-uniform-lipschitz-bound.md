# Vanishing prefactor at one time does not ensure a uniform Lipschitz bound

↑ **Parent:** [Picard-Lindelöf theorem](picard-lindelof-theorem.md)

A coefficient that vanishes at the initial time can hide failure of the uniform [Lipschitz condition](lipschitz-continuity.md) required for an [initial value problem](initial-value-problem.md). For $f(x,y)=x|y|^{2/3}$, the map $y\mapsto f(0,y)$ is identically zero. But every rectangle of positive widths around $(0,0)$ contains some $x\neq0$, and

$$
\frac{|f(x,y)-f(x,0)|}{|y|}=|x||y|^{-1/3}\longrightarrow\infty.
$$

No Lipschitz constant works uniformly on the rectangle. Actual uniqueness also fails: $y=0$ and $y=x^6/216$ are distinct differentiable solutions with initial value zero. Substitution gives $y'=x^5/36=x|y|^{2/3}$ for the second solution. A condition at the single initial time cannot replace control on a neighbourhood.

## ↑ Ancestors (7)

1. [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
