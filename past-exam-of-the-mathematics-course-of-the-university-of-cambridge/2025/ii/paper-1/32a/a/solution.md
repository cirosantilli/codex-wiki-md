<h1 id="32a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A $C^1$ [function](../../../../../../function-split.md) $V$ near an equilibrium at the origin is a [Lyapunov function](../../../../../../lyapunov-function.md) if $V(0)=0$, $V(x)>0$ for $x\ne0$, and

$$
\dot V(x)=\nabla V(x)\cdot f(x)\leq0.
$$

The [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) says these conditions imply stability. The second says that if the last inequality is strict away from the origin, then the origin is asymptotically stable.

To prove the first, fix a sufficiently small ball of radius $\varepsilon$. Positive definiteness and compactness give

$$
m=\min_{|x|=\varepsilon}V(x)>0.
$$

Continuity at zero gives $\delta>0$ such that $|x_0|<\delta$ implies $V(x_0)<m$. Since $V$ cannot increase along a trajectory, that trajectory cannot meet the sphere $|x|=\varepsilon$, where $V\geq m$. It therefore remains in the $\varepsilon$-ball for all forward time, which is stability.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
