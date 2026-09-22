<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The only [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) is $(0,0)$. Its [Jacobian matrix](../../../../../jacobian-matrix.md) is $\begin{pmatrix}-\mu&1\\-1&0\end{pmatrix}$, with [characteristic polynomial](../../../../../characteristic-polynomial.md) $\lambda^2+\mu\lambda+1$. For $\mu>0$ both [eigenvalues](../../../../../eigenvalue.md) have negative real parts, so the origin is locally [asymptotically stable](../../../../../asymptotic-stability.md).

Use the [Lyapunov function](../../../../../lyapunov-function.md) $V=(x^2+y^2)/2$. Along a solution,

$$
\dot V=x\dot x+y\dot y=\mu x^2(x^2/3-1).
$$

A [Lyapunov function](../../../../../lyapunov-function.md) is positive away from the equilibrium and nonincreasing along trajectories; its sufficiently small sublevel sets prove stability. [Asymptotic stability](../../../../../asymptotic-stability.md) additionally means nearby trajectories converge to the equilibrium. The [basin of attraction](../../../../../basin-of-attraction.md) is the set of initial states whose forward solutions exist for all positive time and converge to it. Every closed disc of radius at most $\sqrt3$ is positively invariant, since $\dot V\leq0$ there. The [LaSalle invariance principle](../../../../../lasalle-s-invariance-principle.md) says that a solution in a compact positively invariant set where $\dot V\leq0$ approaches the largest invariant subset of $\{\dot V=0\}$. Here that subset is only the origin: on $x=0$, remaining on the line would require $y=0$; the isolated points $x=\pm\sqrt3,y=0$ on the outer disc do not remain there because $\dot y=-x\ne0$. Hence **the closed disc $x^2+y^2\leq3$ lies in the [basin of attraction](../../../../../basin-of-attraction.md).**

This estimate does not assert that the basin is exactly that disc, or the whole plane. For example, choose $R$ so large that $R^2\geq6(\mu+1)/\mu$ and $R^2>3(\mu+2)/\mu$. The region $x\geq R,\ y\geq-x$ is positively invariant: on $x=R$ one has $\dot x>0$, and on $y=-x$ one has $(x+y)^{\boldsymbol\cdot}=\mu x^3/3-(\mu+2)x>0$. Within it $\dot x\geq\mu x^3/6$, which forces finite-time escape. Thus the attraction is genuinely local. The [Lyapunov function](../../../../../lyapunov-function.md) gives a rigorous sufficient domain for attraction without identifying its entire boundary.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
