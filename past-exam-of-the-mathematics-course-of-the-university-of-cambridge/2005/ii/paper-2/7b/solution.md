<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

A [fixed point](../../../../../fixed-point.md) $x_0$ is [Lyapunov stable](../../../../../lyapunov-stability.md) if for every $\varepsilon>0$ there is $\delta>0$ such that solutions starting within $\delta$ of $x_0$ stay within $\varepsilon$ for all forward times. It has [quasi-asymptotic stability](../../../../../quasi-asymptotic-stability.md) if some neighborhood of $x_0$ consists of initial points whose solutions converge to $x_0$. [Asymptotic stability](../../../../../asymptotic-stability.md) requires both properties.

Choose the [Lyapunov function](../../../../../lyapunov-function.md)

$$
\boxed{V(x,y)=\frac{x^6}{3}+y^2.}
$$

It vanishes only at the origin, is positive elsewhere, and has compact sublevel sets. The vector field is polynomial, hence locally Lipschitz. Along a solution,

$$
\dot V=2x^5(-y-x^3)+2yx^5=-2x^8\leq0.
$$

A small sublevel set is forward invariant and can be fitted inside any prescribed neighborhood, proving [Lyapunov stability](../../../../../lyapunov-stability.md); boundedness also prevents finite-time escape.

For attraction, a bounded forward solution has a nonempty compact limit set, and $V$ decreases to a limit. Every point in that limit set has that same $V$ value. Continuous dependence of solutions makes the limit set forward invariant, so $\dot V=0$ along every trajectory in it. Such a trajectory must have $x=0$ at all times. But then $\dot x=-y$, forcing $y=0$. Thus the only possible limit point is the origin, and every solution converges there. This verifies the invariant-set condition behind the [LaSalle invariance principle](../../../../../lasalle-s-invariance-principle.md), rather than incorrectly treating $\dot V$ as strictly negative at every nonzero point. The origin is therefore **asymptotically stable**, indeed globally attracting.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
