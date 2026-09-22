# Ladder around a right-angled corner

↑ **Parent:** [Lagrange multiplier](lagrange-multiplier.md)

A rigid stick of negligible width can turn horizontally between perpendicular corridors of widths $a,b>0$ precisely when its length does not exceed the displayed value, allowing contact with the walls. A position touching the two outer walls and the inner corner has endpoint intercepts $(a+X,0)$ and $(0,b+Y)$ with $X,Y>0$. Collinearity with the inner corner $(a,b)$ is equivalent to $XY=ab$.

Minimize the squared intercept length $F=(a+X)^2+(b+Y)^2$ under this [optimization constraint](optimization-constraint.md). The [Lagrange multiplier](lagrange-multiplier.md) equations imply $X(a+X)=Y(b+Y)$. Substituting $Y=ab/X$ gives $(X^3-ab^2)(X+a)=0$, so the admissible point is $X=(ab^2)^{1/3}$, $Y=(a^2b)^{1/3}$. There $F=(a^{2/3}+b^{2/3})^3$. Along the positive constraint branch $F$ tends to infinity at both ends and has this one stationary point, proving it is the minimum available clearance over orientations. That minimum is the maximum stick length which can pass through every intermediate orientation.

## ↑ Ancestors (5)

1. [Lagrange multiplier](lagrange-multiplier.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/20/b/solution.md)
