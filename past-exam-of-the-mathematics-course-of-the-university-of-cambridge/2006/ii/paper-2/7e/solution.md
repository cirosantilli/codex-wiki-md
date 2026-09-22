<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

A [strict Lyapunov function](../../../../../strict-lyapunov-function.md) is a [continuously differentiable function](../../../../../continuously-differentiable-function.md) $V$ with $V(0)=0$, $V(x)>0$ off the origin, and $\nabla V\cdot f<0$ off the origin in the domain. Its [compact](../../../../../compact-space.md) [sublevel sets](../../../../../sublevel-set.md) inside the domain are forward invariant and force convergence to the equilibrium. The [domain of stability](../../../../../basin-of-attraction.md), or [basin of attraction](../../../../../basin-of-attraction.md), consists of initial points whose forward solutions exist for all positive time and converge to the [fixed point](../../../../../fixed-point.md).

For $V=(x^2+y^2)/2$, direct differentiation and factorization give

$$
\dot V=-2(x^2+y^2)+x^4+5x^2y^2+4y^4=(x^2+y^2)(-2+x^2+4y^2).
$$

If $R^2=x^2+y^2<1/2$, then $x^2+4y^2\le4R^2<2$, so $\dot V<0$ off zero. For any initial point in that disc, choose a slightly larger [closed disc](../../../../../closed-disc.md) still inside it. The [vector field](../../../../../vector-field.md) points inward on its boundary; the trajectory is bounded, exists globally, and the strict Lyapunov decrease forces its limit to be zero. Thus the origin is [asymptotically stable](../../../../../asymptotic-stability.md) and the whole [open disc](../../../../../open-disc.md) lies in its basin.

If $R^2>2$, then $x^2+4y^2\ge R^2>2$, so $\dot V>0$. A solution starting there cannot cross inward through $R^2=2$ and cannot approach zero. Therefore

$$
\boxed{\{x^2+y^2<1/2\}\subseteq\mathcal B(0)\subseteq\{x^2+y^2\le2\}.}
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
