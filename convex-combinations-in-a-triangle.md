# Convex combinations in a triangle

↑ **Parent:** [Convex combination](convex-combination.md)

Every allocation $(x,y)$ in the [convex feasible region for a resource budget](convex-feasible-region-for-a-resource-budget.md) is a convex combination of its three [extreme points](extreme-point.md):

$$
(x,y)=\lambda_1(0,0)+\lambda_2(6,0)+\lambda_3(0,3),\qquad
\lambda_2=\frac x6,\quad\lambda_3=\frac y3,\quad\lambda_1=1-\frac x6-\frac y3.
$$

The condition $x+2y\leq6$ is exactly $\lambda_1\geq0$; nonnegative $x,y$ give the other two nonnegative [coefficients](coefficient.md). Thus the [half-space](half-space.md) description and the [convex hull](convex-hull.md) description encode the same [triangle](triangle.md). At $(2,1)$ all three [coefficients](coefficient.md) are $1/3$, and at $(3,9/8)$ they are $1/8$, $1/2$, $3/8$. The green and orange points in the budget diagram therefore have two complementary interpretations: direct resource constraints and mixtures of extreme choices.

The three [extreme points](extreme-point.md) alone are not a convex set, because their [midpoints](midpoint.md) are absent. Their [convex hull](convex-hull.md) fills the whole [triangle](triangle.md). More generally, [Caratheodory theorem](caratheodory-s-theorem-convex-hull.md) bounds how many generating points are needed for one convex combination in a finite-dimensional real [vector space](vector-space-split.md); its geometric content is that a complicated collection can describe each attainable average with a short representation.

## ↑ Ancestors (6)

1. [Convex combination](convex-combination.md)
2. [Convex set](convex-set.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
