# Failure of multiplier stationarity at a singular constraint

↑ **Parent:** [Lagrange multiplier](lagrange-multiplier.md)

The nonzero [gradient](gradient.md) condition in the equality [Lagrange multiplier](lagrange-multiplier.md) rule cannot simply be dropped. Minimize $f(x,y)=x$ subject to $g(x,y)=x^2+y^2=0$. The only [feasible point](feasible-point.md) is $(0,0)$, so it is a [global minimum](global-minimum.md) and a [global maximum](global-maximum.md) of $f$ on that [feasible set](feasible-region.md). Nevertheless,

$$
\nabla f(0,0)=(1,0),\qquad\nabla g(0,0)=(0,0),
$$

and no [real number](real-number.md) $\lambda$ satisfies $\nabla f=\lambda\nabla g$. The point is singular for this representation of the [optimization constraint](optimization-constraint.md); the usual [constraint qualification](constraint-qualification.md) fails. The linearized equation $\nabla g\cdot d=0$ permits every direction, even though the actual [feasible set](feasible-region.md) permits no motion at all. This example explains why blindly solving the multiplier equations can miss an optimum.

## ↑ Ancestors (5)

1. [Lagrange multiplier](lagrange-multiplier.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
