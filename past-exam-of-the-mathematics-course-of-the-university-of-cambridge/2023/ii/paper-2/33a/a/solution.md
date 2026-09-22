<h1 id="33a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\dot x=f(x)$, a fixed point $x^*$ satisfies $f(x^*)=0$. It is [Lyapunov stable](../../../../../../lyapunov-stability.md) when, for every $\varepsilon>0$, there is $\delta>0$ such that

$$
|x(0)-x^*|<\delta
\quad\Longrightarrow\quad
|x(t)-x^*|<\varepsilon\quad(t\geq0).
$$

A [Lyapunov function](../../../../../../lyapunov-function.md) on a neighbourhood of $x^*$ is a continuously differentiable function $V$ such that

$$
V(x^*)=0,
\qquad V(x)>0\quad(x\ne x^*),
\qquad
\dot V(x)=\nabla V(x)\cdot f(x)\leq0.
$$

The [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) states that such a function makes $x^*$ Lyapunov stable. If $\dot V<0$ away from $x^*$, then $x^*$ is locally asymptotically stable.

To prove stability, choose a closed ball contained in the domain of $V$. On its boundary sphere $|x-x^*|=\varepsilon$, compactness and positive definiteness give

$$
m=\min_{|x-x^*|=\varepsilon}V(x)>0.
$$

Continuity at $x^*$ supplies $\delta<\varepsilon$ such that $|x-x^*|<\delta$ implies $V(x)<m$. Along a trajectory, $V$ cannot increase. Such a trajectory therefore cannot first reach the boundary sphere, where its value would be at least $m$. This proves Lyapunov stability.

If $\dot V<0$ away from $x^*$, take a sufficiently small compact sublevel set of $V$. The [LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md) says that every trajectory in it approaches the largest invariant subset of $\{\dot V=0\}$, which is just $\{x^*\}$. Hence the equilibrium is also [asymptotically stable](../../../../../../asymptotic-stability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [33A](../../33a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
