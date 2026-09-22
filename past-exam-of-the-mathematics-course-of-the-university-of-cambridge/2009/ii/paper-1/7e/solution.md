<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

A [Lyapunov function](../../../../../lyapunov-function.md) near an equilibrium is a continuously differentiable function with $V(0)=0$, $V(x)>0$ for nonzero nearby $x$, and $\dot V=\nabla V\cdot f\leq0$ along trajectories there. Strict negativity away from the equilibrium gives local [asymptotic stability](../../../../../asymptotic-stability.md). [Lyapunov stability](../../../../../lyapunov-stability.md) itself means that every prescribed small neighborhood contains a smaller neighborhood whose forward trajectories never leave the prescribed one.

For the proposed quadratic form, direct differentiation gives

$$
\dot V=-2[(x-y)^2+(\beta-1)y^2]+4x^2y-2x^3+(2\beta-8)xy^2.
$$

When $\beta>1$, the quadratic part is negative definite, so it dominates the cubic remainder in a sufficiently small ball; $V$ is then a [strict Lyapunov function](../../../../../strict-lyapunov-function.md). If $0<\beta<1$, take $x=y$ to make the leading derivative positive. At $\beta=1$, that same line gives $\dot V=-4x^3$, positive on its negative half. Values $\beta\leq0$ fail positive definiteness of $V$. Therefore

$$
\boxed{\beta>1.}
$$

For $\beta=2$ the full derivative factors, with no small-amplitude truncation:

$$
\dot V=-2(1+x)[(x-y)^2+y^2],\qquad V=x^2+2y^2.
$$

Every closed sublevel set $V\leq c<1$ lies in $x>-1$, is forward invariant, and has strictly decreasing $V$ away from the origin. Compactness and the [Lyapunov stability](../../../../../lyapunov-stability.md) argument therefore show that **the ellipse $x^2+2y^2<1$ belongs to the origin's basin of attraction**. Boundary points with $V=1$ other than $(-1,0)$ also have negative derivative and enter the ellipse. The exception $(-1,0)$ is another [fixed point](../../../../../fixed-point.md), so the largest such sublevel ellipse cannot be included wholesale in the basin. This is a [basin estimate from a Lyapunov sublevel set](../../../../../basin-estimate-from-a-lyapunov-sublevel-set.md), not a claim that no additional points outside the ellipse converge to the origin.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
