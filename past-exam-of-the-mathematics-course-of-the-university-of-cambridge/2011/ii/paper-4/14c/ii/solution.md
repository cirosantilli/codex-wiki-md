<h1 id="14c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the [ellipsoidal Lyapunov function](../../../../../../ellipsoidal-lyapunov-function.md) $V=x^2+2y^2$. Direct substitution of the printed vector field gives

$$
\dot V=2V\bigl[(x-y)^2-1\bigr].
$$

The weighted [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $(x-y)^2\le\tfrac32(x^2+2y^2)=3V/2$, so

$$
\dot V\le-2V(1-3V/2).
$$

For any initial point with $V(0)<2/3$, choose $c$ with $V(0)<c<2/3$. The compact ellipse $V\le c$ is positively invariant, since $\dot V<0$ on its boundary. Inside it,

$$
\boxed{V(t)\le V(0)e^{-2(1-3c/2)t}\longrightarrow0.}
$$

This establishes global forward existence for those trajectories and convergence to the origin, while the [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) establishes stability. **The origin is asymptotically stable and its basin contains $\boxed{x^2+2y^2<2/3}$**. The PDF coefficient in the second equation is $x^2y/2$, with the entire linear term $-x$; placing the factor $1/2$ on the linear term would destroy this factorization.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14C](../../14c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
